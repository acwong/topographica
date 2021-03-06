*********************************************
Reporting specific problems with Topographica
*********************************************

Topographica is used actively in research, and is thus continuously
changing, which inevitably adds new problems as old ones are fixed
and new features are added. When you have found what appears to be a
problem with Topographica itself (whether a bug or a missing
feature), please try the following:

#. If you are using a version that is more than a few weeks old,
   consider trying the most up to date ("bleeding-edge") version via
   `Git`_. The code is updated nearly every day, so by the end of a
   few weeks many changes will have accumulated. Often, bugs will
   have been fixed and new features will have been added already in
   the Git repository, even though they are not yet released
   officially.
#. If the problem is still present in the current version, you can
   search the list of `bug reports`_ on our project pages at GitHub
   to see if we already know about the problem. If you find the
   problem, please feel free to add additional comments to the
   report.
#. We also have a `task list`_, used by the developers to keep track
   of tasks. Try searching this list for information about your
   problem. If you find a related task, please send an e-mail to the
   developer listed as being in charge of that item (if any). If no
   one is yet listed as being responsible, feel free to volunteer!
#. If you can locate where in the code there might be a problem
   (e.g. by going to the line numbers mentioned in a Python
   exception), you will often find a comment with the keyword
   "ALERT" beside the code. These notes are used to mark problems of
   which we are aware but have not yet been able to address. If so,
   please let us know that fixing the problem is urgent, and/or
   suggest fixes for the offending code.
#. Otherwise, please `file a bug report`_. If possible, please
   include:

   -  the full error message, if any
   -  if you are not using Git (i.e. you downloaded a released
      version), please include the Topographica release number (you
      can obtain this by starting Topographica and typing
      ``topo.release``)
   -  if you are using Git, please include the output of
      ``git diff``, ``git status``, and ``git describe``; you can
      create a single file (``report``) containing this information
      with the following command:

      ::

          git describe > report; git status >> report; git diff >> report

   -  which operating system (OS) you are using (Linux, Mac, or
      Windows) and which OS version
   -  any additional file needed to replicate the problem (e.g. a
      script you're using)
   -  a specific recipe (list of steps) that can reproduce the
      problem

   To maximize the speed of resolution, please make sure that your
   problem can be replicated using an unmodified copy of
   Topographica (either released or from Git), and try to have a
   small, clear, quick-to-run example of the problem. Any bug report
   is better than none, so in any case please do send it in even if
   you can't satisfy the above requests. Even so, the clearer and
   simpler it is, the more likely (and more quickly) we will be able
   to address the problem.

#. If you get no reply after a few days, you can try emailing `Jim`_
   directly, in case there was some problem with the email
   notification from the issue tracking system. But it's much more
   effective to use the issue tracking, which automatically delivers
   the appropriate messages to the appropriate developers.

.. _Git: https://github.com/ioam/topographica
.. _bug reports: https://github.com/ioam/topographica/issues?state=open
.. _task list: ../Future_Work/current.html
.. _file a bug report: https://github.com/ioam/topographica/issues/new
.. _Jim: mailto:jbednar@inf.ed.ac.uk?subject=Bug%20report
