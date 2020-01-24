image: alpine
stages:
  - compile  # compile file package.txt from file1 & file2
  - test     # Check correct test in package.txt
  - package  # convert to package.gz
  - delpoy   # copy package.gz to server_DEV via SCP
  -          # connect and run shell         via SSH (inzip, restart)

