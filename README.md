# Validation code for reprocessing AOD from 2011 MinimumBias RAW sample
Run this test in CMS Open Data VM [http://opendata.cern.ch/VM/CMS/2011]
```
cmsrel CMSSW_5_3_32
cd CMSSW_5_3_32/src
cmsenv
git clone https://github.com/katilp/recotest.git

cd recotest
ln -sf /cvmfs/cms-opendata-conddb.cern.ch/FT_53_LV5_AN1_RUNA FT_53_LV5_AN1
ln -sf /cvmfs/cms-opendata-conddb.cern.ch/FT_53_LV5_AN1_RUNA.db FT_53_LV5_AN1_RUNA.db
ls -l
ls -l /cvmfs/
cmsRun configFile.py
```
