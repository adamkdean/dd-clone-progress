#!/bin/bash
#
# Note, this requires pv, get it with:
# $ brew install pv

set -e

clone() {
  local input=$1
  local output=${2:-"clone-$(date +%s).dmg"}
  dd if=$input | pv | dd of=$output
}

clone $1 $2
