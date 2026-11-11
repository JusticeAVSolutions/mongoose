# No workflows on this fork

Cesanta's CI (64 jobs: every vendor board, PPP, s390, armhf, cube examples)
ran on every push to our branches and always failed, because the jobs need
Cesanta's hardware, secrets and mirrors. It burned the org's GitHub Actions
minutes for nothing.

This fork is consumed as a submodule by fw-net-core, whose own CI (host
tests, sanitizers, fuzzing, HIL) exercises the code we actually ship. Test
changes to this fork through fw-net-core.
