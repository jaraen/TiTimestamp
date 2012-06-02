Ti.LogTimestamp
===========================================

This is a Titanium mobile module for iOS that helps reading and measuring performance and execution times.

Provides two methods for your experimentation. In both cases, time stamp is returned/printed as a double type representing number of seconds with six decimal (0.000000), aka microseconds (10^-6), since 00:00:00 1 January 2001.

::
	-(void)logTimeStamp

logs the timestamp in console.

::
	-(id)getTimeStamp

returns the timeStamp as value.


Both methods have been implemented in the most simplest way to avoid interfere in execution, but small typecasting operations are required (since these operations are always the same, I think is ok to compare different performance methods this way). 

I'm trying to figure out if getTimeStamp should use Titanium macro ENSURE_UI_THREAD, by now I haven't find a good reason to do it.


USING YOUR MODULE IN CODE
-------------------------

see example/app.js file

AUTHOR
-------
Javier Rayon

twitter: @jrayon

Contact: javier at criteriastudio dot com

GitHub Repo: https://github.com/jaraen

Appcelerator DevLink: http://developer.appcelerator.com/devlink/profile/1190171/javier-rayon


LICENSE
--------
Copyright (c) 2012 Javier Rayon

::
	Permission is hereby granted, free of charge, to any person obtaining a copy
	of this software and associated documentation files (the "Software"), to deal
	in the Software without restriction, including without limitation the rights
	to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
	copies of the Software, and to permit persons to whom the Software is
	furnished to do so, subject to the following conditions:

	The above copyright notice and this permission notice shall be included in
	all copies or substantial portions of the Software.

	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
	FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
	AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
	LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
	THE SOFTWARE.	
