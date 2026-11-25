# Exercise 15. Comparing Directions Using the Cosine of the Angle

## Given Vectors

We are given:

$$
a=(1,2,1)
$$

$$
b=(2,4,2)
$$

$$
c=(2,0,3)
$$

We need to calculate the cosine for each pair, order the pairs by increasing angle, and explain why the value for a and b is 1.

## Solution

### 1. Calculating the Lengths

First, I calculate the lengths of all vectors.

For a:

$$
|a|=\sqrt{1^2+2^2+1^2}
=\sqrt6
$$

For b:

$$
|b|=\sqrt{2^2+4^2+2^2}
=\sqrt{24}
$$

For c:

$$
|c|=\sqrt{2^2+0^2+3^2}
=\sqrt{13}
$$

### 2. Calculating the Cosine for Each Pair

I use the formula:

$$
\cos\theta=\frac{u\cdot v}{|u||v|}
$$

**Pair 1: a and b**

First, I calculate the dot product:

$$
a\cdot b=1(2)+2(4)+1(2)
$$

$$
=2+8+2=12
$$

Now I calculate the cosine:

$$
\cos\theta=\frac{12}{\sqrt6\sqrt{24}}
$$

$$
=\frac{12}{12}=1
$$

Therefore:

$$
\boxed{\cos\theta=1}
$$

**Pair 2: a and c**

First, I calculate the dot product:

$$
a\cdot c=1(2)+2(0)+1(3)
$$

$$
=2+0+3=5
$$

Now:

$$
\cos\theta=\frac{5}{\sqrt6\sqrt{13}}
$$

Therefore:

$$
\boxed{\cos\theta=\frac5{\sqrt{78}}}
$$

**Pair 3: b and c**

First, I calculate the dot product:

$$
b\cdot c=2(2)+4(0)+2(3)
$$

$$
=4+0+6=10
$$

Now:

$$
\cos\theta=\frac{10}{\sqrt{24}\sqrt{13}}
$$

$$
=\frac{10}{2\sqrt{78}}
$$

Therefore:

$$
\boxed{\cos\theta=\frac5{\sqrt{78}}}
$$

### 3. Ordering the Pairs by Increasing Angle

The cosine values are:

- For a and b: 1
- For a and c: 5/√78
- For b and c: 5/√78

A larger cosine means a smaller angle.

Therefore, the order from the smallest angle to the largest angle is:

1. a and b (0°)
2. a and c (approximately 55.5°)
3. b and c (approximately 55.5°)

The last two pairs have the same angle.

### 4. Why Is the Value for a and b Equal to 1?

We can see that:

$$
b=(2,4,2)=2(1,2,1)
$$

So:

$$
b=2a
$$

This means that both vectors have the same direction, but different lengths.

Their angle is 0 degrees, so the cosine is 1.

## Conclusion

The cosine values are:

$$
\cos(a,b)=1
$$

$$
\cos(a,c)=\frac5{\sqrt{78}}
$$

$$
\cos(b,c)=\frac5{\sqrt{78}}
$$

Vectors a and b have the same direction because b is twice a. This is why their cosine value is 1, even though their lengths are different.