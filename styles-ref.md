# Data Types

### int
```
int = [0..9]^(1+) 
      0
      100
```

### float
```
float = option (-) [0..9]^(1+) option (.[0..9]^(1+)) option (f)
        1
        2.0f
        2.f
        -0.2f
```

### color


```
color =  4 * float
         #fff                 //white     
         #fffe                //with alpha-channel
         (r, g, b)            //(1, 1, 1) or (255, 255, 255)
         (r, g, b, a)         //(1, 1, 1, 0.1) or (255, 255, 255, 25)
```

### vector4 
```
vector4 = 10                 // (10, 10, 10, 10)
          10, 20             // (10, 20, 10, 20)
          10, 20, 30, 40     // (left, top, right, bottom)
```

# Attributes

### width
```
    = width: int 
      width: 100
```
### height
```
    = height: int 
      height: 100
```
### margin
```
    = margin: vector4
      margin: 10 
      margin: -10 0 0 0
      margin: 10 20 
```

### padding

see #margin #vector4

### color

set text color
```
    = color: color
      color: #fff
      color: #fffe
      color: (1, 1, 1)
      color: (1, 1, 1, 0.1)
      color: (255, 0, 0)
```

### bg-color

set the background color, see #color, mutiple with bg-image (if present)

### bg-image

set the background image, mutiple with bg-color (if present)

### layout

how child items are placed in the current item

```
   layout: 
           | vert 
           | horz 
           | grid (cols, cell_width, cell_height, space_width, space_height)
```

### grow

define the ability for a item to grow if there is free space

```
    grow: 1  //don't care 
```
