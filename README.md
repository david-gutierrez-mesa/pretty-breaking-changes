A simple script that searches for commits with a keyword to identify breaking changes, generating a markdown report.

To use the script, you need to pass following parameters:

* repo_path = the path to your repository
* branch = the branch you want to use in the repo entered in repo_path
* start_hash = the start of the range of commits to consider
* end_hash = the end of the range of commits to consider. This is the only optional parameter. If you don't enter it HEAD is going to be used as end_hash

Example:

    ./pretty-breaking-changes-markdown.py /home/yo/src/liferay-portal-ee master f63d698232b7b620536bb32f854286b132fcc07a 4a2e75e4e6fd4c225db62f303ccc33cdd1782ba4
