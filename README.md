# VariableFinder #

VariableFinder is a TRIPS module that finds world modeling variables or the codes used to fill them given a sequence of words describing them.

This file is the README for the standalone version of VariableFinder. The main documentation in the file [README](README) is written in the context of TRIPS. For the standalone version, `$TRIPS_BASE` is `trips/`.

## Build instructions ##

    ./configure [--with-python=/path/to/python] [--with-pip=/path/to/pip]
    make
    make install # installs to trips/etc/ and trips/bin/

## Run instructions ##

For standalone usage, you should give VariableFinder the `-connect no` option, t prevent it from trying to connect to the TRIPS Facilitator:

    ./trips/bin/VariableFinder -connect no

Then it will accept requests on its standard input stream, and give replies on its standard output stream (in addition to a few startup messages you can ignore). For the details of these requests and replies, see the file [README](README).

## Licensing ##

VariableFinder is licensed using the [GPL 2+](http://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html) (see `LICENSE.txt`):

VariableFinder - resolves references to world modeling variables/codes
Copyright (C) 2018  Institute for Human & Machine Cognition

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
