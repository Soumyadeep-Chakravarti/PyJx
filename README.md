# PyJx

**PyJx** is a Python library designed to give seamless, Pythonic access to Java classes and methods. Inspired by JNI, PyJx allows Python developers to call Java functions, interact with objects, and exchange data across runtimes with minimal boilerplate. The goal is to make cross-language development intuitive while maintaining performance and memory safety.

> ⚠️ **Development Status:** Alpha / In Progress. PyJx is actively being developed. APIs may change, and internal memory handling is involved. Use with caution; it is not production-ready.

---

## 🚀 Key Features

* **Pythonic Java Access:** Call Java classes and methods as if they were native Python objects.
* **Zero Boilerplate:** No Java glue code required; import classes and invoke methods directly.
* **Stable Memory Handling:** Built on PyProbe for safe, low-level memory access and pointer stability.
* **Cross-Language Interop:** Exchange data efficiently between Python and Java.
* **Flexible Data Support:** Handles primitives, objects, and custom structures.

---

## 📌 Usage Example

```python
from pyjni.imports import MathUtils

# Call a Java method like a normal Python function
result = MathUtils.add(2, 3)
print(result)  # Outputs: 5
```

You can also import full packages:

```python
from pyjni.imports import family

person = family.Person("Alice")
print(person.greet())  # Calls Java method internally
```

---

## 🛠️ Development Notes

* PyJx runs entirely on the Python side.
* A running JVM is required for Java integration.
* The project is in early alpha; expect API changes and breaking updates.
* Contributions and experiments are welcome, but stability is not guaranteed.
