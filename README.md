# www.ec2instances.info-ec2op

Catalog of EC2 prices per instance type.

This data was exported as CSV from https://ec2instances.info then stripped down and saved as JSON files.



## Usage

To fetch the json file directly into javascript (with CORS enabled):

```
https://cdn.jsdelivr.net/gh/autofitcloud/www.ec2instances.info-ec2op/www.ec2instances.info/t3b_smaller_familyL2.json
```

To read in python as a pandas dataframe with [`read_json`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html):

```
pip3 install isitfit

from isitfit.utils import ec2_catalog
df = ec2_catalog()
df.shape
# (261, 2)
```

Source code for `isitfit.utils.ec2_catalog` is available [here](https://github.com/autofitcloud/isitfit/blob/master/isitfit/utils.py#L38)


## Created with

[git-remote-aws](https://git-remote-aws.autofitcloud.com)

```
git remote add r1_aws_ec2catalog aws+ec2::/catalog
git fetch r1_aws_ec2catalog
echo "www.ec2instances.info/t0_raw.json" > .gitignore
git add .gitignore
git add www.ec2instances.info
git commit -am 'first commit'
```


## License

Check file `LICENSE` (MIT License similar to https://github.com/powdahound/ec2instances.info/)
