# Dummy_Updata_On_DVC
mkdir -p workspace//Dummy_Updata_On_DVC 
cd workspace/Dummy_Updata_On_DVC/
git init
dvc cache dir workspace/Dummy_Updata_On_DVC
dvc init
git add train.py
dvc add Test.zip
dvc run -d unzip -q Test.zip
git add .
git commit -m 'test'
git branch -M master
git remote add origin https://github.com/vviettinh/Dummy_Updata_On_DVC.git
git push origin master
