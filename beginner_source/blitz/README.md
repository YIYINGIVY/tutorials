## Reproduce this result

#### Reproduce
```bash
git checkout aimev2
git checkout 0a17bf77367927869323716d61a343b298e900a0
curl https://www.mltrack.ml/api/rest/v1/git/get-patch?experimentKey=8bfeeedb5a904ed38b989e4e8380a885 -H"Authorization: 34K0NbIdl05WON1C832tRydMt" > patch.zip
unzip patch.zip
git apply git_diff.patch
```

#### Run
```
/opt/conda/bin/python /workspace/pytorch/image_moderation/AIMEv2/model_training/src/main.py --t text
```
