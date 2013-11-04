cpu_governor
============

CPU usage limiting, primarily for LTSP systems.

Runaway processes can be a problem in LTSP systems. I've found in particular that Adobe's 
Acrobat Reader, Firefox, and flash can easily get out of control and suck up 100% of a processor. 
The cpulimit command (available in Ubuntu and Debian) can limit individual processes by intermittently 
forcing them to sleep. This program (cpu_governor) monitors specified processes for excessive cpu usage.
If a monitored process exceeds the specified cpu usage range, then it will be restrained by the cpulimit
command.

The cpulimit program is an independent binary which should be available in your distribution.

This version of cpu_governor was written a few years ago and has some issues. I'm using it as-is for a starting
point for a hopefully more accurate and thorough version.

=====================

LICENSE AND COPYRIGHT

Copyright (C) 2013 Steve Cayford

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see L<http://www.gnu.org/licenses/>.

