# jsondir2graphql

Generate graphql type definitions from a directory of json files using [@walmartlabs/json-to-simple-graphql-schema](https://github.com/walmartlabs/json-to-simple-graphql-schema)

## Usage

```sh
npx jsondir2graphql test/fixtures/ test/schema/schema.graphql
```

## Example

#### Input

foo.json

```js
{
    "foo": "1"
}
```

bar.json

```js
{
    "bar": "1"
}
```

#### Output

schema.graphql

```js
type Foo {
  foo: String
}
type Bar {
  bar: String
}
```

### Notes

Requires Node 14 for top level await and ES modules.
