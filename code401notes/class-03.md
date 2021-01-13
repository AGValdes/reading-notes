# Class 03: System.I.O

## File and Stream I/O
**File and stream I/O (input/output):**  the transfer of data either to or from a storage medium
- In .NET, contain types that: enable reading and writing on data streams and files, perform compression and decompression on files, enable communication through pipes and serial ports.
**Common file and directory classes:**
- **File**:provides static methods for creating, copying, deleting, moving, and opening files, and helps create a FileStream object.

-**FileInfo**:provides instance methods for creating, copying, deleting, moving, and opening files, and helps create a FileStream object.

- **Directory**:provides static methods for creating, moving, and enumerating through directories and subdirectories.

- **DirectoryInfo**: provides instance methods for creating, moving, and enumerating through directories and subdirectories.

- **Path**: provides methods and properties for processing directory strings in a cross-platform manner.
**Streams** involve 3 operations:
- Reading: transfering data from a stream into a data structure, EX: an array of bytes
- Writing: transferring data to a stream from a data source.
- Seeking: querying and modifying the current position within a stream.
**Commonly used stream classes:**
- **FileStream:** for reading and writing to a file.

= **IsolatedStorageFileStream**: for reading and writing to a file in isolated storage.

- **MemoryStream**" for reading and writing to memory as the backing store.

- **BufferedStream**: for improving performance of read and write operations.

- **NetworkStream**: for reading and writing over network sockets.

- **PipeStream**: for reading and writing over anonymous and named pipes.

- **CryptoStream**: for linking data streams to cryptographic transformations.
**Commonly used REader and Writer CLasses:**
- BinaryReader and BinaryWriter: for reading and writing primitive data types as binary values.

- StreamReader and StreamWriter: for reading and writing characters by using an encoding value to convert the characters to and from bytes.

- StringReader and StringWriter: for reading and writing characters to and from strings.

- TextReader and TextWriter: serve as the abstract base classes for other readers and writers that read and write characters and strings, but not binary data.
**Async I/O operations:**
- Reading or writing a large amount of data should be done asynchronously asynchronously if your application needs to remain responsive to the user. 
- asynchronous members contain Async in their names EX: CopyToAsync, FlushAsync, ReadAsync, and WriteAsync

- **Compression:**the process of reducing the size of a file for storage.
- **Isolated Storage:**a data storage mechanism that provides isolation and safety by defining standardized ways of associating code with saved data.

## How to Write a File
**Classes and methods to write text to file:**
- **StreamWriter** contains methods to write to a file synchronously **Write and WriteLine** or asynchronously **WriteAsync and WriteLineAsync**.

- **File** provides static methods to write text to a file, such as **WriteAllLines and WriteAllText**, or to append text to a file, such as **AppendAllLines, AppendAllText, and AppendText**.

- **Path** is for strings that have file or directory path information. It contains the **Combine** method and, in .NET Core 2.1 and later, the **Join** and **TryJoin** methods, which allow concatenation of strings to build a file or directory path.

## Read to a File
[Code Example: how to create an empty file stream, write data to it, and read data from it.](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file)
