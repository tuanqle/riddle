This is a command-line program demonstrating the `Water Jug Riddle` solution.

`Water Jug Riddle` in simple term is by using only an X-gallon and Y-gallon jug (no third jug),
to measure Z-gallon of water.

### Installation

```
    git clone https://github.com/tuanqle/riddle.git
```

### Building

```
    cd riddle
    docker build -t riddle-app .
```

### Running
```
   docker run -it riddle-app
```

### Input

The app takes 3 values on 1 line separated by space.

__Example__
```
$docker run -it riddle-app
Water Jug Riddle
Enter value for X, Y, and Z (where X,Y,Z is number of gallon): 3 5 2
```

#### What it does?

As the program starts, it asks user to input 3 integer values for X, Y, and Z which represent
number of gallons for: Jug X, Jug Y, and the measurement Z-gallon. It validates these values
for errors. It uses recursive algorithm to find the measurment Z-gallon. If found, it will out
steps to derive the result.

### Contents

    `README.md`    - This README file
    `main.go`      - main program
    `main_test.go` - unit test code
