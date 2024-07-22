Coding styleguides


## Naming Conventions
### Variables
camelCase: Typically used for variable names. - I will recommend this to distinguish variables from functions
 - Example: crossSection, eventNumber, trackMomentum
snake_case: Sometimes used, especially in more script-like or older codebases.
 - Example: cross_section, event_number, track_momentum

### Functions and Methods
camelCase: Commonly used for function names.
 - Example: calculateEnergy(), processEvent(), readDataFile()
snake_case: Less common, but can be found in some codebases. - I will recommend this since in ROOT the main function should be the same as the filename (which should be snake_case)
 - Example: calculate_energy(), process_event(), read_data_file()

### Constants
ALL_CAPS_SNAKE_CASE: Used for constants and macro definitions.
 - Example: MAX_TRACKS, PI, SPEED_OF_LIGHT

### Classes and Structs
PascalCase: Used for class and struct names.
 - Example: EventProcessor, DataAnalysis, ParticleTrack

### Filenames
snake_case: Commonly used for filenames.
 - Example: event_processor.cpp, data_analysis.h, particle_track.h

### Namespaces
lowercase: Often used for namespaces.
 - Example: namespace cms, namespace atlas



## Indentation 
3 spaces, not a tab.
### Braces and Spaces: 
Usually this...
```cpp
if (x is true) {
   we do y
}
```
Functions should be...
```cpp
int function (int x)
{
   body of function
}
```
if you have a continuation of the same statement use the following...
```cpp
if (x == y) {
   ...
} else if (x > y) {
   ...
} else {
   ...
}
```

## Declarations
pointer '*' shoudl go with the variable name rather than the type.
``` char *t ```
to ensure that mutliple variable will be assigned correctly, e.g.
``` char *t, *u, *v ```


## Whitespace
A long string of conditional operators should be split onto separate lines.
```
   if (foo->next==NULL && totalcount<needed && needed<=MAX_ALLOT
    && server_active(current_input)) { ...
Might be better as
   if (foo->next == NULL
    && totalcount < needed && needed <= MAX_ALLOT
    && server_active(current_input))
   {
    ...
```

# Python things

If a file is meant to be used as an executable, its main functionality should be in a main() function, and your code should always check if __name__ == '__main__' before executing your main program, so that it is not executed when the module is imported.

```python
def main():
    ...

if __name__ == '__main__':
    main()
```
