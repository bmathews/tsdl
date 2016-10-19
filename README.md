Tsdl — Thin bindings to SDL for OCaml
-------------------------------------------------------------------------------
v0.9.1

Tsdl is an OCaml library providing thin bindings to the cross-platform
SDL C library.

Tsdl depends on the [SDL 2.0.1][sdl] C library (or later),
[ocaml-ctypes][ctypes] and the `result` compatibility package.
Tsdl is distributed under the BSD3 license.

[sdl]: http://www.libsdl.org/
[ctypes]: https://github.com/ocamllabs/ocaml-ctypes

Home page: http://erratique.ch/software/tsdl  
Contact: Daniel Bünzli `<daniel.buenzl i@erratique.ch>`


## Installation

Tsdl needs the C library SDL 2.0.1 or later installed on your
system. Tsdl can be installed with `opam`:

    opam install tsdl

If you don't use `opam` consult the [`opam`](opam) file for
build instructions and a complete specification of the dependencies.


## Documentation

The documentation and API reference is automatically generated by
from the source interfaces. It can be consulted [online][online] 
or via `opkg doc tsdl`.

[online]: http://erratique.ch/software/tsdl/doc/


## Sample programs

Sample programs are located in the `test` directory of the
distribution. They can be built with:

    ocamlbuild -use-ocamlfind tests.otarget

The resulting binaries are in `_build/test` :

- `test.native`, tests the bindings, the executable should exit 
   with 0.
- `sdlevents.native`, traces SDL events.
- `min.native` a minimal SDL example.
