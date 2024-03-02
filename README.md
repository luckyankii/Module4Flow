**SomeContract**

This contract defines a struct called `SomeStruct` with four variables (`a`, `b`, `c`, `d`) and three functions (`publicFunc`, `contractFunc`, `privateFunc`). It also defines a resource called `SomeResource` with one variable (`e`) and one function (`resourceFunc`). The contract provides a function `createSomeResource()` to create an instance of `SomeResource`, and a function `questsAreFun()` that can be called from any area.

**Areas**

The contract divides code into four areas:

- **AREA 1**: Inside `SomeStruct.structFunc()`, `init()`
- **AREA 2**: Inside `SomeResource.resourceFunc()`
- **AREA 3**: Inside `questsAreFun()`
- **AREA 4**: script part

**Variable Access**

The variables can be read and written to in the following areas:

- **a**: Read in AREA 1, 2, 3. Written in AREA 1.
- **b**: Read in all areas. Written in AREA 1.
- **c**: Read in AREA 1, 2. Written in AREA 1.
- **d**: Read in AREA 1. Written in AREA 1.

**Function Calls**

The functions can be called from:

- **publicFunc**: All areas.
- **contractFunc**: AREA 1, 2.
- **privateFunc**: AREA 1.
