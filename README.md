## TBC (Tcl ByteCode) decoder

The .tbc file is generated by Tcl Pro. This repo try to add comments on .tbc file and disassemble .tbc file for human reading.

### Example

``` go
func ExampleEncode() {
    src := []byte("proc")
    dst := make([]byte, 150)
    length := Encode(dst, src)
    fmt.Printf("%s", dst[:length])
    // Output:
    // ,CHr@
}
```
### reference
 - ActiveState Teapot [cmpWrite.c](https://github.com/ActiveState/teapot/blob/master/lib/tclcompiler/cmpWrite.c)

