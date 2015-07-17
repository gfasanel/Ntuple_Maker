# Ntuple_Maker
IIHE Ntuple Maker

Usercode/IIHETree/src

IIHEAnalysis e' il contenitore di tutti i moduli

in IIHETree c'e' un BuildFile.xml che serve per dire quali moduli di CMSSW importare

DataFormats/MuonReco

Per cercare le cose `lxr cms fnal` su google

Per aggiungere un modulo

* In src/IIHEModuleExample.cc e manda Example in Tau
* In interface/IIHEModuleExample.h e manda Example in Tau
* In interface/IIHEAnalysis.h e cerca Tau
* In IIHE.py aggiungi la tua collezione

A questo punto

cmsRun IIHE.py (questo e' fuori da Usercode)

Considera che nel .cc quando fai "store" gli dici "fai Fill nel tree"

quando hai fatto, compila con

`scram b -j4`
