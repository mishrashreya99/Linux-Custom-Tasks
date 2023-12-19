
.\" Man page for internsctl
.TH INTERNSCTL 1 "2023-12-19" "v0.1.0" "internsctl manual"
.SH NAME
internsctl \- Custom Linux command for operations
.SH SYNOPSIS
.B internsctl
[\fIOPTION\fR] [\fICOMMAND\fR] [\fIARGUMENTS\fR]
.SH DESCRIPTION
This manual page documents the internsctl command, a custom Linux command for various operations.
.P
\fBinternsctl\fR is a versatile command-line tool with different commands and options.
.SH COMMANDS
The following commands are available:
.IP \fBcpu getinfo\fR
Display CPU information.
.IP \fBmemory getinfo\fR
Display memory information.
.IP \fBuser create <username>\fR
Create a new user with the specified username.
.IP \fBuser list [--sudo-only]\fR
List regular users, optionally only those with sudo permissions.
.IP \fBfile getinfo [OPTIONS] <file-name>\fR
Get information about a file.
.SH OPTIONS
.IP \fB--version\fR
Display the command version.
.IP \fB--help\fR
Display help information.
.SH EXAMPLES
Display CPU information:
.IP
.B internsctl cpu getinfo
.IP
Create a new user:
.IP
.B internsctl user create john_doe
.IP
Get information about a file's size:
.IP
.B internsctl file getinfo --size myfile.txt
.SH SEE ALSO
.BR lscpu (1),
.BR free (1),
.BR useradd (8),
.BR passwd (1),
.BR stat (1)
.SH AUTHOR
Written by Your Name.
.SH COPYRIGHT
This is free software; see the source for copying conditions.
.SH BUGS
Report bugs to Your Email.
