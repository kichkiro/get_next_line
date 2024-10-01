<img src="https://github.com/kichkiro/42/blob/assets/banner_get_next_line.jpg?raw=true" width="100%"/>

# Get Next Line

<i>
	<p>
		This project is about programming a function that returns a line read from a file descriptor.
	</p>
</i>

#### <i>[subject](_subject/en.subject.pdf) v.10</i>

<details>
<summary><i><b>Project Structure  📂</b></i></summary>

```js
├── README.md
├── LICENSE
├── project
│   ├── get_next_line_bonus.c
│   ├── get_next_line_bonus.h
│   ├── get_next_line.c
│   ├── get_next_line.h
│   ├── get_next_line_utils_bonus.c
│   └── get_next_line_utils.c
└── _subject
    └── en.subject.pdf
```
</details>

## 📌 - Key Topics

### File Descriptors
Understanding file descriptors is crucial for reading data in C. 
Each file descriptor represents an open file, socket, or other input/output resource, and it is managed by the operating system. 
The get_next_line function relies on the read() system call, which reads data from the specified file descriptor into a buffer. 
Mastery of file descriptor handling allows for efficient line-by-line reading from files and standard input.

### Static Variables
Static variables maintain their value between function calls, making them essential for tracking the state of the reading process in the get_next_line function. 
When dealing with multiple calls to get_next_line(), a static variable can store the buffer's state across these calls, enabling the function to return subsequent lines of input. 
Proper use of static variables is key to implementing a robust solution without using global variables, adhering to best practices in C programming.

## 🛠️ - Usage

``` sh
git clone https://github.com/kichkiro/get_next_line.git
cd get_next_line/
```
It's now possible to use the get_next_line() function by including the header files and source files.

The function prototype is __char *get_next_line(int fd);__

## ⚖️ - License

See [LICENSE](LICENSE)
