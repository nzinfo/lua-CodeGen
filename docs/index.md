
*Perfection is achieved, not when there is nothing more to add,
but when there is nothing left to take away.
<br /> &mdash; Antoine de Saint-Exupéry*

## Overview

lua-CodeGen is a "safe" template engine.

lua-CodeGen enforces a strict Model-View separation. Only 4 primitives are supplied :

- attribute reference,
- template include,
- conditional include,
- and template application (i.e., _map_ operation).

lua-CodeGen allows to split template in small chunk,
and encourages the reuse of them by inheritance.

Each chunk of template is like a rule of a grammar for an _unparser generator_.

lua-CodeGen is not dedicated to HTML, it could generate any kind of textual code.

## References

The Terence Parr's articles :

- [Enforcing Strict Model-View Separation in Template Engines](http://www.cs.usfca.edu/~parrt/papers/mvc.templates.pdf)
- [A Functional Language For Generating Structured Text](http://www.cs.usfca.edu/~parrt/papers/ST.pdf)

Note : lua-CodeGen is not a port of Terence Parr's
[StringTemplate](http://www.stringtemplate.org/).

[Lust](http://github.com/weshoke/Lust) is another Lua module based on
[StringTemplate](http://www.stringtemplate.org/).

## Status

lua-CodeGen is in beta stage.

It's developed for Lua 5.1, 5.2 & 5.3.

## Download

lua-CodeGen source can be downloaded from
[GitHub](http://github.com/fperrad/lua-CodeGen/releases/).

## Installation

Two variants are available, a pure Lua without dependency and a
[LPeg](http://www.inf.puc-rio.br/~roberto/lpeg/lpeg.html) based.

lua-CodeGen is available via LuaRocks:

    luarocks install lua-codegen
    # luarocks install lua-codegen-lpeg

or manually, with:

    make install.lua
    # make install.lpeg

## Test

The test suite requires the module
[lua-TestMore](http://fperrad.github.io/lua-TestMore/).

    make test.lua
    # make test.lpeg

## Copyright and License

Copyright © 2010-2014 François Perrad
[![OpenHUB](http://www.openhub.net/accounts/4780/widgets/account_rank.gif)](http://www.openhub.net/accounts/4780?ref=Rank)
[![LinkedIn](http://www.linkedin.com/img/webpromo/btn_liprofile_blue_80x15.gif)](http://www.linkedin.com/in/fperrad)

This library is licensed under the terms of the MIT/X11 license,
like Lua itself.
