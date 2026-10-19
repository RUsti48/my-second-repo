# Листинги команд для работы с файлами в Linux

## Листинг команды touch
```bash
root@roman-VB:/home/roman/repo/my-second-repo# touch --help
Update the access and modification times of each FILE to the current time.

Usage: touch [OPTION]... [FILE]...

Arguments:
  [files]...  

Options:
      --help              Print help information.
  -a                      change only the access time
  -t <STAMP>              use [[CC]YY]MMDDhhmm[.ss] instead of the current time
  -d, --date <STRING>     parse argument and use it instead of current time
  -f                      (ignored)
  -m                      change only the modification time
  -c, --no-create         do not create any files
  -h, --no-dereference    affect each symbolic link instead of any referenced
                          file (only for systems that can change the timestamps
                          of a symlink)
  -r, --reference <FILE>  use this file's times instead of the current time
      --time <WORD>       change only the specified time: "access", "atime", or
                          "use" are equivalent to -a; "modify" or "mtime" are
                          equivalent to -m [possible values: atime, mtime]
  -V, --version           Print version

