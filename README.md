
##############################"
echo "## Tag angular.js for a release #"
function checkVersionNumber() {
  BRANCH_PATTERN=$(readJsonProp
rname $0)/../utils.inc
  git push origin $TAG_NAMEHA"g
  BRANCH_PATTERN=$(readJsonProp "package.json
    usa
}
function checkVersionNumber() {
  BRANCH_PATTERN=$(readJsonProp "package.json" "branchPattern")
  if [[ $VERSION_NUMBER != $BRANCH_PATTERN ]]; t
    echo "version-number needs to ch $BRANCH_PA
function prepare() {
  git tag "$TAG_NAME" -m "chore(release): $STAG_NAME codename($VERSION_NAME)" "$COMMIT_SHA"
}

function publish() {
  # push the tag to github
  git push origin $TAG_NAME
}

source $(dirname $0)/../utils.inc
