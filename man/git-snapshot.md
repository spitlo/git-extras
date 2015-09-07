git-snapshot(1) -- Show file contents at a given point in time
===============================================

## SYNOPSIS

`git-snapshot` [&lt;file&gt; &lt;date&gt; &lt;lookback&gt;]

## DESCRIPTION

Shows the entire content of a specified file at a given point in time

## OPTIONS

  &lt;file&gt;

  The name of the file to show.

  &lt;date&gt;

  The point in time, in format YYYY-MM-DD.

  &lt;lookback&gt;

  Number of days to go back looking for

## EXAMPLES

 Defining a new alias:

    $ git snapshot last "cat-file commit HEAD"

 Providing only one argument, `git-alias` searchs for aliases matching the given value:

    $ git alias ^la
    last = cat-file commit HEAD

 `git-alias` will show all aliases if no argument is given:

    $ git alias
    s = status
    amend = commit --amend
    rank = shortlog -sn --no-merges
    whatis = show -s --pretty='tformat:%h (%s, %ad)' --date=short
    whois = !sh -c 'git log -i -1 --pretty="format:%an <%ae>

## AUTHOR

Written by spitlo

## REPORTING BUGS

&lt;<https://github.com/spitlo/git-extras/issues>&gt;

## SEE ALSO

&lt;<https://github.com/spitlo/git-extras>&gt;
