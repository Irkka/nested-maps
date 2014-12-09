# nested-maps adds some utility functions to manage nested sass maps with ease


## Example usage

```
@import 'nested-maps';

$nested-map: (
hello: (
  world: (
      name: 'This',
      occupation: 'is'
    ),
  foo: 'a nested map'
  ),
  f: (
    yeaah: 'hell yeah'
  )
);

$another-nested-map: (
hello: (
  world: (
    age: 5,
    occupation: 'no'
  ),
  foo: 'an another nested map'
  )
);

@debug $nested-map;
@debug $another-nested-map;
@debug nested-map-merge($nested-map, $another-nested-map);
```
