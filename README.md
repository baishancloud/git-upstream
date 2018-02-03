# git-upstream

Manage upstream git repos.

It depends on a configure file ".gitupstream" at git repo root dir.

## Install:

Copy this script to a dir in PATH.

## Configure

Configure file ".gitupstream" syntax:

    <upstream_name_1>     <upstream_url_1>
    <upstream_name_2>     <upstream_url_2>
    ...

Example:

    > cat .gitupstream
    chriswolfvision     git@github.com:chriswolfvision/eplot.git


With above config, "git upstream" will:

-   Add missing remote.
-   Try to set-url for each upstream.
-   fetch -p the upstream repo.
