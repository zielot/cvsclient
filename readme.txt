Modified version of Michael Clarke's patched cvsclient to require that Jsch ssh connection use a username and password by default instead of a SSH key. 

Michael's patched version of the Netbeans CvsClient incorporated changes to support the following:
1. Maven build (change project structure and added pom.xml)
2. Add serialization (supports sending work to slaves for Jenkins builds)
3. Synchronize DateFormat calls and shared variables (supports concurrent jobs using CVS)
4. Move SshConnection from external Netbeans library into CvsClient to support ext connections

All changes are provided under the original licenses of the CVS client (GPL or CCDL) - see the header
notices in individual files for details.

CvsClient makes use of the JSCH library to allow SSH communication for CVS ext connections. The
JSCH library is released under a BSD style license:

Copyright (c) 2002-2011 Atsuhiko Yamanaka, JCraft,Inc. 
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

  1. Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.

  2. Redistributions in binary form must reproduce the above copyright 
     notice, this list of conditions and the following disclaimer in 
     the documentation and/or other materials provided with the distribution.

  3. The names of the authors may not be used to endorse or promote products
     derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED ``AS IS'' AND ANY EXPRESSED OR IMPLIED WARRANTIES,
INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL JCRAFT,
INC. OR ANY CONTRIBUTORS TO THIS SOFTWARE BE LIABLE FOR ANY DIRECT, INDIRECT,
INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
