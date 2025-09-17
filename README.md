# @discere-os/flann.wasm

WebAssembly port of FLANN - Fast Library for Approximate Nearest Neighbors with SIMD optimization and machine learning capabilities.

[![CI/CD](https://github.com/discere-os/discere-nucleus/actions/workflows/flann-wasm-ci.yml/badge.svg)](https://github.com/discere-os/discere-nucleus/actions)
[![JSR](https://jsr.io/badges/@discere-os/flann.wasm)](https://jsr.io/@discere-os/flann.wasm)
[![npm version](https://badge.fury.io/js/@discere-os%2Fflann.wasm.svg)](https://badge.fury.io/js/@discere-os%2Fflann.wasm)
[![License](https://img.shields.io/badge/License-BSD--3--Clause-blue.svg)](COPYING)
[![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://github.com/discere-os/discere-nucleus)





FLANN - Fast Library for Approximate Nearest Neighbors
======================================================

FLANN is a library for performing fast approximate nearest neighbor searches in high dimensional spaces. It contains a collection of algorithms we found to work best for nearest neighbor search and a system for automatically choosing the best algorithm and optimum parameters depending on the dataset.
FLANN is written in C++ and contains bindings for the following languages: C, MATLAB, Python, and Ruby.


Documentation
-------------

Check FLANN web page [here](http://www.cs.ubc.ca/research/flann).

Documentation on how to use the library can be found in the doc/manual.pdf file included in the release archives.

More information and experimental results can be found in the following paper:

  * Marius Muja and David G. Lowe, "Fast Approximate Nearest Neighbors with Automatic Algorithm Configuration", in International Conference on Computer Vision Theory and Applications (VISAPP'09), 2009 [(PDF)](https://www.cs.ubc.ca/research/flann/uploads/FLANN/flann_visapp09.pdf) [(BibTex)](http://people.cs.ubc.ca/~mariusm/index.php/FLANN/BibTex)


Getting FLANN
-------------

If you want to try out the latest changes or contribute to FLANN, then it's recommended that you checkout the git source repository: `git clone git://github.com/mariusmuja/flann.git`

If you just want to browse the repository, you can do so by going [here](https://github.com/mariusmuja/flann).


Conditions of use
-----------------

FLANN is distributed under the terms of the [BSD License](https://github.com/mariusmuja/flann/blob/master/COPYING).

Bug reporting
-------------

Please report bugs or feature requests using [github's issue tracker](http://github.com/mariusmuja/flann/issues).


## 💖 Support This Work

This WebAssembly port is part of a larger effort to bring professional desktop applications to browsers with native performance.

**👨‍💻 About the Maintainer**: [Isaac Johnston (@superstructor)](https://github.com/superstructor) - Building foundational browser-native computing infrastructure through systematic C/C++ to WebAssembly porting.

**📊 Impact**: 70+ open source WASM libraries enabling professional applications like Blender, GIMP, and scientific computing tools to run natively in browsers.

**🚀 Your Support Enables**:
- Continued maintenance and updates
- Performance optimizations
- New library ports and integrations
- Documentation and tutorials
- Cross-browser compatibility testing

**[💖 Sponsor this work](https://github.com/sponsors/superstructor)** to help build the future of browser-native computing.
