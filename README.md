# www.ec2instances.info-csv

exported and stripped down csv files from ec2instancse.info Used in ec2op-osi


## Usage

Can be used from browser with CORS using

```
https://cdn.jsdelivr.net/gh/autofitcloud/www.ec2instances.info-ec2op/www.ec2instances.info/t3b_smaller_familyL2.json
```

The file is 118kB


## Created with

```
git remote add r1_aws_ec2catalog aws+ec2::/catalog
git fetch r1_aws_ec2catalog
echo "www.ec2instances.info/t0_raw.json" > .gitignore
git add .gitignore
git add www.ec2instances.info
git commit -am 'first commit'
```
