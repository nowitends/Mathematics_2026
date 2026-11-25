# Exercise 3. Vector Normalization

## Given Vector

We are given:

$$
v=(3,4)
$$

We need to find a unit vector with the same direction and orientation. Then we check its length and reconstruct the original vector.

## Solution

### 1. Calculate the Length of v

First, I calculate the length of the vector:

$$
|v|=\sqrt{3^2+4^2}
$$

$$
=\sqrt{9+16}
$$

$$
\boxed{|v|=5}
$$

### 2. Find the Unit Vector

To get a unit vector, I divide the original vector by its length:

$$
e=\frac{v}{|v|}
$$

$$
e=\frac{(3,4)}{5}
$$

Therefore:

$$
\boxed{e=\left(\frac35,\frac45\right)}
$$

### 3. Check That the Length Is 1

I calculate the length of the new vector:

$$
|e|=\sqrt{\left(\frac35\right)^2+
\left(\frac45\right)^2}
$$

$$
=\sqrt{\frac9{25}+\frac{16}{25}}
$$

$$
=\sqrt{\frac{25}{25}}
$$

$$
\boxed{|e|=1}
$$

So the new vector is a unit vector.

### 4. Reconstruct the Original Vector

We use the formula:

$$
v=|v|\cdot e
$$

Substituting the values:

$$
v=5\left(\frac35,\frac45\right)
$$

$$
=(3,4)
$$

This gives the original vector.

### 5. What Changes During Normalization?

During normalization, the length of the vector changes from 5 to 1.

However, its direction and orientation stay the same because we divide both components by the same positive number.

## Conclusion

The unit vector is:

$$
\boxed{e=\left(\frac35,\frac45\right)}
$$

Its length is 1, and multiplying it by the original length gives back the vector:

$$
\boxed{v=(3,4)}
$$

Normalization changes the length but keeps the direction and orientation.