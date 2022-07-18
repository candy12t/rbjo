# rbjo

## Usage
```shell
$ rbjo key=value
{"key":"value"}
```

```shell
$ rbjo name=candy12t age=23
{"name":"candy12t","age":23}
```

```shell
$ rbjo -p name=candy12t age=23
{
  "name": "candy12t",
  "age": 23
}
```

```shell
$ rbjo -a A B C
["A","B","C"]
```

```
$ rbjo -p key1=value1 obj=`rbjo key2=value2`
{
  "key1": "value1",
  "obj": {
    "key2": "value2"
  }
}
```

```
$ rbjo -p name=candy12t age=23 skill=`rbjo -a Go Ruby Vim Shell`
{
  "name": "candy12t",
  "age": 23,
  "skill": [
    "Go",
    "Ruby",
    "Vim",
    "Shell"
  ]
}
```
