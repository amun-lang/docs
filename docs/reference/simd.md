SIMD (Single Instruction Multiple Data) instruction is a type of computer instruction that allows a single instruction to operate on multiple pieces of data in parallel. SIMD instructions are used to perform repetitive calculations on large amounts of data, such as those found in multimedia applications, scientific simulations, and data processing tasks.

SIMD instructions provide a powerful tool for accelerating certain types of computations in a wide range of applications, and their support by modern CPUs and programming languages has made them increasingly accessible to developers.

In Amun you can take the advantage of SIMD concept using the Vector type for example you can apply Arithmetic, Comparions, Logical operators like any other permittive 

### Declaring Vector type

Vector type is almost the same as Static Size Array type but prefixed with @vec, but note that vector type supports only unsigned integers and floats only and you can't create multi dimentions vector.

```
var u8_vec : @vec[3]uint8 = @vec[1_u8, 2_u8, 3_u8];
var u16_vec : @vec[3]uint16 = @vec[1_u16, 2_u16, 3_u16];
var u32_vec : @vec[3]uint32 = @vec[1_u32, 2_u32, 3_u32];
var u64_vec : @vec[3]uint64 = @vec[1_u64, 2_u64, 3_u64];

var f32_vec : @vec[3]float32 = @vec[1_f32, 2_f32, 3_f32];
var f64_vec : @vec[3]float64 = @vec[1_f64, 2_f64, 3_f64];
```

### Count attribute for Vector type

In Amun you can easily get the length of the vector like array or string using `count` attribute

```
var u8_vec : @vec[3]uint8 = @vec[1_u8, 2_u8, 3_u8];
var length = u8_vec.count;
```

### For each on Vector type

In Amun you can iterate over vector type like array or string

```
var vec = @vec[1_u8, 2_u8, 3_u8];
for (vec) {
    printf("vec[%d] = %u\t", it_index, it);
}
```