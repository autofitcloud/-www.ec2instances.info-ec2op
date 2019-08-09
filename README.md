# www.ec2instances.info-csv

exported and stripped down csv files from ec2instancse.info Used in ec2op-osi


## Created with

```
git remote add r1_aws_ec2catalog aws+ec2::/catalog
git fetch r1_aws_ec2catalog
echo "www.ec2instances.info/t0_raw.json" > .gitignore
git add .gitignore
git add www.ec2instances.info
git commit -am 'first commit'
```