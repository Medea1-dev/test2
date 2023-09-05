
##############################"
echo "## Tag angular.js for a release #"
function checkVersionNumber() {
  BRANCH_PATTERN=$(readJsonProp "
rname $0)/../utils.inc
  git push origin $TAG_NAMEHA"github
source $(dirname $0)/../utils.in
  BRANCH_PATTERN=$(readJsonProp "package.json" "branchPat
    echo "version-number needs to match $BRANCH_PATTERN on this brch"
    usage
  fi
}
function checkVersionNumber() {
  BRANCH_PATTERN=$(readJsonProp "package.json" "branchPattern")
  if [[ $VERSION_NUMBER != $BRANCH_PATTERN ]]; then
    echo "version-number needs to match $BRANCH_PATTERN on this branch"
    usage
  fi
}

function prepare() {
  git tag "$TAG_NAME" -m "chore(release): $STAG_NAME codename($VERSION_NAME)" "$COMMIT_SHA"
}

function publish() {
  # push the tag to github
  git push origin $TAG_NAME
}

source $(dirname $0)/../utils.inc
