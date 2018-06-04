---
Description: A 4x4 matrix that contains methods and operator overloads.
ms.assetid: c354d28b-bb08-41c5-bb59-90a912181f0f
title: D3DXMATRIX structure
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: structure
ms.date: 05/31/2018
---

# D3DXMATRIX structure

A 4x4 matrix that contains methods and operator overloads.

## Syntax


```C++
typedef struct D3DXMATRIX {
  FLOAT _ij;
} D3DXMATRIX, *LPD3DXMATRIX;
```



## Members

<dl> <dt>

**\_ij**
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/windows/desktop/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

</dd> <dd>

The (i, j) component of the matrix, where i is the row number and j is the column number. For example, \_34 means the same as \[a₃₄\], the component in the third row and fourth column.

</dd> </dl>

## Remarks

C programmers cannot use the D3DXMATRIX structure, they must use the D3DMATRIX structure. C++ programmers can take advantage of overloaded constructors and assignment, unary, and binary (including equality) operators.

In D3DX, the \_34 element of a projection matrix cannot be a negative number. If your application needs to use a negative value in this location, it should scale the entire projection matrix by -1 instead.

### D3DXMATRIX Extensions

**D3DXMATRIX** has the following C++ extensions.


```
#ifdef __cplusplus
typedef struct D3DXMATRIX : public D3DMATRIX
{
public:
    D3DXMATRIX() {};
    D3DXMATRIX( CONST FLOAT * );
    D3DXMATRIX( CONST D3DMATRIX&amp; );
    D3DXMATRIX( CONST D3DXFLOAT16 * );
    D3DXMATRIX( FLOAT _11, FLOAT _12, FLOAT _13, FLOAT _14,
                FLOAT _21, FLOAT _22, FLOAT _23, FLOAT _24,
                FLOAT _31, FLOAT _32, FLOAT _33, FLOAT _34,
                FLOAT _41, FLOAT _42, FLOAT _43, FLOAT _44 );


    // access grants
    FLOAT&amp; operator () ( UINT Row, UINT Col );
    FLOAT  operator () ( UINT Row, UINT Col ) const;

    // casting operators
    operator FLOAT* ();
    operator CONST FLOAT* () const;

    // assignment operators
    D3DXMATRIX&amp; operator *= ( CONST D3DXMATRIX&amp; );
    D3DXMATRIX&amp; operator += ( CONST D3DXMATRIX&amp; );
    D3DXMATRIX&amp; operator -= ( CONST D3DXMATRIX&amp; );
    D3DXMATRIX&amp; operator *= ( FLOAT );
    D3DXMATRIX&amp; operator /= ( FLOAT );

    // unary operators
    D3DXMATRIX operator + () const;
    D3DXMATRIX operator - () const;

    // binary operators
    D3DXMATRIX operator * ( CONST D3DXMATRIX&amp; ) const;
    D3DXMATRIX operator + ( CONST D3DXMATRIX&amp; ) const;
    D3DXMATRIX operator - ( CONST D3DXMATRIX&amp; ) const;
    D3DXMATRIX operator * ( FLOAT ) const;
    D3DXMATRIX operator / ( FLOAT ) const;

    friend D3DXMATRIX operator * ( FLOAT, CONST D3DXMATRIX&amp; );

    BOOL operator == ( CONST D3DXMATRIX&amp; ) const;
    BOOL operator != ( CONST D3DXMATRIX&amp; ) const;

} D3DXMATRIX, *LPD3DXMATRIX;

#else //!__cplusplus
typedef struct _D3DMATRIX D3DXMATRIX, *LPD3DXMATRIX;
#endif //!__cplusplus
        
```



## Requirements



|                   |                                                                                         |
|-------------------|-----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>D3DX10Math.h</dt> </dl> |



## See also

<dl> <dt>

[D3DX Structures](d3d10-graphics-reference-d3dx10-structures.md)
</dt> </dl>

 

 



