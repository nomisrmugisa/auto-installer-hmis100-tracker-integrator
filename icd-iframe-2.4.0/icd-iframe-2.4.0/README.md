#### How To
> Run command below
```sh
DHIS2_VERSION="{dhis2_version}" && \
USERNAME="{username}" && \
TOKEN="{token}" && \
REPO="{repo}" && \
rm -rf updates && \
url="https://$USERNAME:$TOKEN@github.com/$REPO.git" && \
git clone -b "$DHIS2_VERSION" "$url" updates && \
cd updates && \
./update.sh "$DHIS2_VERSION" "$USERNAME" "$TOKEN" "$REPO"

```
> e.g.
```sh
DHIS2_VERSION="2.40" && \
USERNAME="dhis2scripts" && \
TOKEN="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" && \
REPO="dhis2scripts/icdiframe" && \
rm -rf updates && \
url="https://$USERNAME:$TOKEN@github.com/$REPO.git" && \
git clone -b "$DHIS2_VERSION" "$url" updates && \
cd updates && \
./update.sh "$DHIS2_VERSION" "$USERNAME" "$TOKEN" "$REPO"

```
