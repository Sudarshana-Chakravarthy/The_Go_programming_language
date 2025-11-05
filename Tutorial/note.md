# 1.1 Hello World


- Go is a compiled language. The Go toolcahin converts the sourceprogram and the things it depends on into instructions in the native machine language of a computer.

- These tools are accessed through a single command called go that has a number of subcommands. The simplest of these subcommands is `run` which compiles the source code from one or more source files, links it with libraries, then runs the resulting executable file.

	- **`go run helloworld.go`**

- If you want to compile and save the compiled result for later use, we use **`build`**.

	- **`go build helloworld.go`**

- This creates an executable binary file called helloworld that can be run anytime without further processing.

	- **`./helloworld`**

- In every programming language first code will always be printing hello world. The below code is written in go.

```go
package main
	
import "fmt"
	
func main(){

fmt.Println("Hello, World")

}
```

## Working of the program

- Go code is organized into packages, which are similar to libraries or modules in other languages. 

- Each source file begins with a **`package`** declaration, here **package main**,that states which package the file belongs to, followed by a list of other packages that it imports, and then the declarations of the program thatare stored in that file.

- Package main is special. It defines a standalone executable program, not alibrary. Within **`package main`** the **`function main`** is also special — Rt’s where execution of the program begins. Whatever main does is what the program does. Of course, main will normally call up on functions in other packages to do much of the work,such as the function **fmt.Println**.

- 
