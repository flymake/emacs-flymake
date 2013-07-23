* flymake.el 0.4.16 (2013-05-19-01:30)
  * Pull upstream patch for non-writable dirs.
    (Prodding provided by @rrthomas, patch originally by Stefan Monnier.)
  * Also don't run on unreadable dirs (ie, before you get chance to M-x make-directory.)

* flymake.el 0.4.15 (2013-02-12-20:02)
  * Remove accidental commit of debugging skip of file cleanup.

* flymake.el 0.4.14 (2013-02-08-20:21)
  * Properly escape CHK_SOURCES filenames for the shell in C/C++ syntax checkers.

* flymake.el 0.4.13 (2012-10-28-23:19)
  * Use -e option to xmlstarlet XML validation so that line errors are captured and
    exit code doesn't disable flymake.
    (Contributed by @marcinant.)

* flymake.el 0.4.12 (2012-07-23-09:29)
  * Use file-truename in flymake-create-temp-inplace to ensure tempfile names are in normal form.
    (Contributed by @arnested.)

* flymake.el 0.4.11 (2012-06-03-00:29)
  * Added flymake-stop-syntax-check to stop syntax checks in a single buffer.
  * Added flymake-restart-syntax-check to stop syntax checks in a single buffer and start new one.

* flymake.el 0.4.10 (2012-05-23-14:50)
  * Fix error regexp for gcc 4.5+ on windows.
    (Contributed by @abbec.)

* flymake.el 0.4.9 (2012-03-28-06:22)
  * Use file-truename to ensure tempfile names are in normal form.
    (Contributed by @arnested.)

* flymake.el 0.4.8 (2012-03-22-07:47)
  * Merge in upstream changes from GNU Emacs version.
    * Doc fixes for minor-mode: http://bzr.savannah.gnu.org/lh/emacs/trunk/revision/107172.
  * No functional changes.

* flymake.el 0.4.7 (2012-02-07-09:15)
  * Add support for rpm specfiles with rpmlint. (Contributed by Adrian Likins.)
  * Add support for gettext po files with msgfmt. (Contributed by Adrian Likins.)

* flymake.el 0.4.6 (2012-01-01-09:25)
  * Add support for csslint.
  * Update DOCSTRING for the various temp filename functions.
  * Attempt to find Perl project include dir if it's in a standard place.
  * Fix temp-dir prefix stripping in flymake-delete-temp-directory.

* flymake.el 0.4.5 (2011-11-26-19:28)
  * Use butlast for error truncation rather than messing with car/cdr directly.
  * Clarify use of $PERLBREW_ROOT to detect if perlbrew sync is required.
  * Add support for info class error messages.
    (Inspired by https://github.com/gabrielelanaro/emacs-for-python/)
  * Customizable error-message classification regexps.
  * Add support for Javascript errors with jshint.

* flymake.el 0.4.4 (2011-11-01-21:37)
  * No longer prompt about running flymake processes when killing buffers.
    (Karl Chen via http://lists.gnu.org/archive/html/emacs-devel/2010-03/msg01217.html)
  * Attempt to prevent MOTD/login message from remote Tramp syntax checks
    appearing at the end of the buffer being syntax-checked.
  * Suppress Tramp message-area spam during remote syntax checks.
  * Enable flymake logging to message area again.

* flymake.el 0.4.3 (2011-10-19-20:49)
  * Fix interaction of tramp with flymake-run-in-place set to nil.
    (Thanks to @nullie and @dncohen for analysis of the problem and debugging.)

* flymake.el 0.4.2 (2011-10-16-07:02)
  * Add support for multiple errors in error tooltip. (Contributed by nullie.)
  * Control number of errors in tooltip with flymake-number-of-errors-to-display.
