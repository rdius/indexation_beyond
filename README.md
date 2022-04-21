## indexation_beyond

#### Please, provide the data-examples folder with these files: 

```
-   relations = "./data-examples/relations.full.tsv/relations_min.tsv"
-   BioNLP_onto = './data-examples/BioNLP-OST+EnovFood.txt'
-   taxid_microorganisms = './data-examples/taxid_microorganisms.tsv/taxid_microorganisms.tsv'
```
Build the Jsonl file by calling :

```
beyond_db_preprocess(relations,BioNLP_onto,taxid_microorganisms)
```
Index Data to ES using Logstash

```
sudo /usr/share/logstash/bin/logstash -f 'beyond_conf.conf' #manage to give the absolute path
```
