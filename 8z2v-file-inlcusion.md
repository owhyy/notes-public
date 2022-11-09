---
title: File Inclusion Exploit
created: 2022-10-09
keywords: [Hacking]
---

> Being able to read files like `get.php?file=/var/...` _because there is no input validation_

- If having write access to `/tmp`, you can have [[zczf-remote-command-executio|Remote command execution]]
- Sometimes input may be filtered, so you can only have .php files. You can use `%00` (IF PHP <5.3.4) or the `/.`(current directory)
- Sometimes there is input validation (replacing `./` with a '', for example). We have to be smarter than the validation (for that example, we can do `./..//` which will translate to `./`, or `..//..//` _for PHP's filter_)
- You can also have Remote File Inclusion, where you get a malicious file from your server and it gets executed on the target server
