# Exercise 5. Relative Position of Two Lines

## Given

We are given two lines:

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1)
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1)
$$

We need to check if they intersect, are parallel, or are skew.

## Solution

### 1. Finding the Coordinates

For the first line:

$$
x=1+t,\quad y=1+2t,\quad z=t
$$

For the second line:

$$
x=2,\quad y=s,\quad z=1-s
$$

### 2. Checking the Intersection

I compare the coordinates:

$$
1+t=2 \Rightarrow t=1
$$

From the z-coordinate:

$$
t=1-s
$$

$$
1=1-s \Rightarrow s=0
$$

Now I check the y-coordinate:

$$
1+2(1)=0
$$

$$
3\neq 0
$$

So, the coordinates do not give the same point.

The lines do not intersect.

### 3. Checking if They Are Parallel

The direction vectors are:

$$
v_1=(1,2,1)
$$

$$
v_2=(0,1,-1)
$$

These vectors are not scalar multiples of each other.

Therefore, the lines are not parallel.

## Conclusion

The lines do not intersect and their direction vectors are not parallel.

Therefore:

$$
\boxed{\text{The lines are skew.}}
$$