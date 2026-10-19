# Листинги команд для работы с файлами в Linux

## Листинг команды touch
```bash
root@roman-VB:/home/roman/repo/my-second-repo# touch --help

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
  -V, --version           Print version```

## Листинг команды cat
```bash
root@roman-VB:/home/roman/repo/my-second-repo# cat --help
Concatenate FILE(s), or standard input, to standard output
With no FILE, or when FILE is -, read standard input.

Usage: cat [OPTION]... [FILE]...

Options:
  -A, --show-all          equivalent to -vET
  -b, --number-nonblank   number nonempty output lines, overrides -n
  -e                      equivalent to -vE
  -E, --show-ends         display $ at end of each line
  -n, --number            number all output lines
  -s, --squeeze-blank     suppress repeated empty output lines
  -t                      equivalent to -vT
  -T, --show-tabs         display TAB characters at ^I
  -v, --show-nonprinting  use ^ and M- notation, except for LF (\n) and TAB (\t)
  -u                      (ignored)
  -h, --help              Print help
  -V, --version           Print version

## Листинг команды nano
```bash
root@roman-VB:/home/roman/repo/my-second-repo# nano --help
Использование: nano [ОПЦИИ] [[+СТРОКА[,СТОЛБЕЦ]] ФАЙЛ]…

Чтобы поместить курсор на определённую строку файла, введите номер
и «+» перед именем файла. Номер столбца можно ввести после запятой.
Когда задано имя файла «-», то nano читает данные со стандартного ввода.

 Опция          Длинная опция           Значение
 -A             --smarthome             Включить умную кнопку home
 -B             --backup                Сохранять резервные копии существующих файлов
 -C <каталог>   --backupdir=<каталог>   Каталог для хранения уникальных резервных копий
 -D             --boldtext              Использовать жирный шрифт
 -E             --tabstospaces          Преобразовать табуляции в пробелы
 -F             --multibuffer           По умолчанию читать файл в новый буфер
 -G             --locking               Использовать файлы блокировки (как в vim)
 -H             --historylog            Сохранить и загрузить старые строки поиска/замены
 -I             --ignorercfiles         Не использовать на файлы nanorc
 -J <число>     --guidestripe=<число>   Показать линейку на этом столбце
 -K             --rawsequences          Исправлять проблему малой клавиатуры
 -L             --nonewlines            Не добавлять пустую строку в конце
 -M             --trimblanks            Обрезать хвостовые пробелы при ручном переносе строк
 -N             --noconvert             Не преобразовывать из DOS/Mac формата
 -O             --bookstyle             Ведущий пробел означает новый параграф
 -P             --positionlog           Сохранить и восстановить расположение курсора
 -Q <regex>     --quotestr=<regex>      Регулярное выражение для поиска кавычек
 -R             --restricted            Ограничить доступ к файловой система
 -S             --softwrap              Переносить длинные строки при просмотре
 -T <число>     --tabsize=<число>       Установить ширину табуляции
 -U             --quickblank            Очищать строку состояние при нажатии
 -V             --version               Показать версию и выйти
 -W             --wordbounds            Использовать более точное определение границ слов
 -X <строка>    --wordchars=<строка>    Какие еще символы являются частью слова
 -Y <имя>       --syntax=<имя>          Использовать описание синтаксиса для подсветки
 -Z             --zap                   Очищать выделенную область с помощью Bsp и Del
 -a             --atblanks              Делать мягкий перенос только на пробелах
 -b             --breaklonglines        Жестко переносить слишком длинные строки
 -c             --constantshow          Постоянно показывать позицию курсора
 -d             --rebinddelete          Исправить проблему Backspace/Delete
 -e             --emptyline             Не занимать строку под строкой заголовком
 -f <файл>      --rcfile=<файл>         Использовать только этот файл для настроек nano
 -g             --showcursor            Показывать курсор и текст справки в файловом менеджере
 -h             --help                  Показать этот текст и выйти
 -i             --autoindent            Автоматический отступ на новых строках
 -j             --jumpyscrolling        Прокрутка по пол-экрана, а не по строке
 -k             --cutfromcursor         Вырезать от курсора до конца строки
 -l             --linenumbers           Показывать номера строк перед текстом
 -m             --mouse                 Разрешить использование мыши
 -n             --noread                Не читать файл (только писать его)
 -o <каталог>   --operatingdir=<каталог>Установить рабочий каталог
 -p             --preserve              Зарезервировать кнопки XON (^Q) и XOFF (^S)
 -q             --indicator             Показать индикатор позиции+части
 -r <число>     --fill=<число>          Установить ширину для жесткого переноса и выравнивания
 -s <программа> --speller=<программа>   Использовать эту альтернативную проверку правописания
 -t             --saveonexit            Не спрашивая сохранять изменения при выходе
 -u             --unix                  По умолчанию сохранять файл в Unix формате
 -v             --view                  Режим просмотра (только чтение)
 -w             --nowrap                Не переносить длинные строки [по умолчанию]
 -x             --nohelp                Не показывать две строки помощи внизу
 -y             --afterends             Останавливаться на краях слов при зажатом Ctrl+Right
 -z             --listsyntaxes          Показать список доступных синтаксисов
 -@             --colonparsing          Принять нотацию 'имяфайла:номерстроки'
 -%             --stateflags            Показывать состояния в строке заголовка
 -_             --minibar               Показать панель обратной связи внизу
 -0             --zero                  Скрыть все панели и развернуть терминал
 -/             --modernbindings        Использовать известные сочетания клавиш

## Листинг команды pwd
```bash
root@roman-VB:/home/roman/repo/my-second-repo# pwd --help
pwd: pwd [-LP]
    Print the name of the current working directory.
    
    Options:
      -L	print the value of $PWD if it names the current working
    		directory
      -P	print the physical directory, without any symbolic links
    
    By default, `pwd' behaves as if `-L' were specified.
    
    Exit Status:
    Returns 0 unless an invalid option is given or the current directory
    cannot be read.

## Листинг команды ls
```bash
root@roman-VB:/home/roman/repo/my-second-repo# ls --help
List directory contents.
Ignore files and directories starting with a '.' by default

Usage: ls [OPTION]... [FILE]...

Options:
      --help
          Print help information.
      --format <format>
          Set the display format.
  -C
          Display the files in columns.
  -l, --long
          Display detailed information.
  -x
          List entries in rows instead of in columns.
  -T, --tabsize <COLS>
          Assume tab stops at each COLS instead of 8 [env: TABSIZE=]
  -m
          List entries separated by commas.
      --zero
          List entries separated by ASCII NUL characters.
  -D, --dired
          generate output designed for Emacs' dired (Directory Editor) mode
      --hyperlink[=<WHEN>]
          hyperlink file names WHEN [default: never] [possible values: always, auto, never]
  -1
          List one file per line.
  -o
          Long format without group information.
          Identical to --format=long with --no-group.
  -g
          Long format without owner information.
  -n, --numeric-uid-gid
          -l with numeric UIDs and GIDs.
      --quoting-style <quoting-style>
          Set quoting style. [possible values: literal, locale, shell, shell-escape, shell-always,
          shell-escape-always, clocale, c, escape]
  -N, --literal
          Use literal quoting style. Equivalent to `--quoting-style=literal`
  -b, --escape
          Use escape quoting style. Equivalent to `--quoting-style=escape`
  -Q, --quote-name
          Use C quoting style. Equivalent to `--quoting-style=c`
  -q, --hide-control-chars
          Replace control characters with '?' if they are not escaped.
      --show-control-chars
          Show control characters 'as is' if they are not escaped.
      --time <field>
          Show time in `<field>`:
          access time (-u): atime, access, use;
          change time (-t): ctime, status.
          modification time: mtime, modification.
          birth time: birth, creation;
  -c
          If the long listing format (e.g., -l, -o) is being used, print the
          status change time (the 'ctime' in the inode) instead of the modification
          time. When explicitly sorting by time (--sort=time or -t) or when not
          using a long listing format, sort according to the status change time.
  -u
          If the long listing format (e.g., -l, -o) is being used, print the
          status access time instead of the modification time. When explicitly
          sorting by time (--sort=time or -t) or when not using a long listing
          format, sort according to the access time.
      --hide <PATTERN>
          do not list implied entries matching shell PATTERN (overridden by -a or -A)
  -I, --ignore <PATTERN>
          do not list implied entries matching shell PATTERN
  -B, --ignore-backups
          Ignore entries which end with ~.
      --sort <field>
          Sort by `<field>`: name, none (-U), time (-t), size (-S), extension (-X) or width [possible values:
          name, none, time, size, version, extension, width]
  -S
          Sort by file size, largest first.
  -t
          Sort by modification time (the 'mtime' in the inode), newest first.
  -v
          Natural sort of (version) numbers in the filenames.
  -X
          Sort alphabetically by entry extension.
  -U
          Do not sort; list the files in whatever order they are stored in the
          directory.  This is especially useful when listing very large directories,
          since not doing any sorting can be noticeably faster.
  -L, --dereference
          When showing file information for a symbolic link, show information for the
          file the link references rather than the link itself.
      --dereference-command-line-symlink-to-dir
          Do not follow symlinks except when they link to directories and are
          given as command line arguments.
  -H, --dereference-command-line
          Do not follow symlinks except when given as command line arguments.
  -G, --no-group
          Do not show group in long format.
      --author
          Show author in long format. On the supported platforms,
          the author always matches the file owner.
  -a, --all
          Do not ignore hidden files (files with names that start with '.').
  -A, --almost-all
          In a directory, do not ignore all file names that start with '.',
          only ignore '.' and '..'.
  -f
          List all files in directory order, unsorted. Equivalent to -aU. Disables --color unless explicitly
          specified.
  -d, --directory
          Only list the names of directories, rather than listing directory contents.
          This will not follow symbolic links unless one of `--dereference-command-line
          (-H)`, `--dereference (-L)`, or `--dereference-command-line-symlink-to-dir` is
          specified.
  -h, --human-readable
          Print human readable file sizes (e.g. 1K 234M 56G).
  -k, --kibibytes
          default to 1024-byte blocks for file system usage; used only with -s and per
          directory totals
      --si
          Print human readable file sizes using powers of 1000 instead of 1024.
      --block-size <BLOCK_SIZE>
          scale sizes by BLOCK_SIZE when printing them
  -i, --inode
          print the index number of each file
  -r, --reverse
          Reverse whatever the sorting method is e.g., list files in reverse
          alphabetical order, youngest first, smallest first, or whatever.
  -R, --recursive
          List the contents of all directories recursively.
  -w, --width <COLS>
          Assume that the terminal is COLS columns wide.
  -s, --size
          print the allocated size of each file, in blocks
      --color[=<color>]
          Color output based on file type. [possible values: always, auto, never]
      --indicator-style <indicator-style>
          Append indicator with style WORD to entry names:
          none (default),  slash (-p), file-type (--file-type), classify (-F) [possible values: none, slash,
          file-type, classify]
  -F, --classify[=<when>]
          Append a character to each file name indicating the file type. Also, for
          regular files that are executable, append '*'. The file type indicators are
          '/' for directories, '@' for symbolic links, '|' for FIFOs, '=' for sockets,
          '>' for doors, and nothing for regular files. when may be omitted, or one of:
              none - Do not classify. This is the default.
              auto - Only classify if standard output is a terminal.
              always - Always classify.
          Specifying --classify and no when is equivalent to --classify=always. This will
          not follow symbolic links listed on the command line unless the
          --dereference-command-line (-H), --dereference (-L), or
          --dereference-command-line-symlink-to-dir options are specified. [possible values: always, auto, never]
      --file-type
          Same as --classify, but do not append '*'
  -p
          Append / indicator to directories.
      --time-style <TIME_STYLE>
          time/date format with -l; see TIME_STYLE below [env: TIME_STYLE=]
      --full-time
          like -l --time-style=full-iso
  -Z, --context
          print any security context of each file
      --group-directories-first
          group directories before files; can be augmented with
          a --sort option, but any use of --sort=none (-U) disables grouping
  -V, --version
          Print version


## Листинг команды head
```bash
root@roman-VB:/home/roman/repo/my-second-repo# head --help
Print the first 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.
With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.

Usage: head [OPTION]... [FILE]...

Arguments:
  [FILE]...  [default: -]

Options:
  -c, --bytes <[-]NUM>   print the first NUM bytes of each file;
                         with a leading '-', print all but the last
                         NUM bytes of each file
  -n, --lines <[-]NUM>   print the first NUM lines instead of the first 10;
                         with a leading '-', print all but the last
                         NUM lines of each file
  -q, --quiet            never print headers giving file names [alias: --silent]
  -v, --verbose          always print headers giving file names
  -z, --zero-terminated  line delimiter is NUL, not newline
  -h, --help             Print help
  -V, --version          Print version

## Листинг команды tail
```bash
root@roman-VB:/home/roman/repo/my-second-repo# head --help
Print the first 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.
With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.

Usage: head [OPTION]... [FILE]...

Arguments:
  [FILE]...  [default: -]

Options:
  -c, --bytes <[-]NUM>   print the first NUM bytes of each file;
                         with a leading '-', print all but the last
                         NUM bytes of each file
  -n, --lines <[-]NUM>   print the first NUM lines instead of the first 10;
                         with a leading '-', print all but the last
                         NUM lines of each file
  -q, --quiet            never print headers giving file names [alias: --silent]
  -v, --verbose          always print headers giving file names
  -z, --zero-terminated  line delimiter is NUL, not newline
  -h, --help             Print help
  -V, --version          Print version

## Листинг команды less
```bash
root@roman-VB:/home/roman/repo/my-second-repo# less README.md 
