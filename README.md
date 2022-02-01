Info about used software (e.g. environment.yml, Dockerfile): https://github.com/nf-core/proteomicslfq

Instructions:

* Install Java 8+
* Install docker or singularity
* Install nextflow (`wget -qO- https://get.nextflow.io | bash`)
* ~/nextflow run nf-core/proteomicslfq -r dev -profile docker --input https://raw.githubusercontent.com/bigbio/proteomics-metadata-standard/master/annotated-projects/PXD001819/PXD001819.sdrf.tsv --database https://raw.githubusercontent.com/wombat-p/Transproteomic-Pipeline/dev/Results/yeast_UPS.fasta  --add_decoys
 -with-report -with-trace -with-timeline

Results:

* MSstats folder contains final results/quants post-processed by MSstats
* openms\_msstats-ready\_out.csv contains the raw aggregated intensities

Note: PRIDE changed the access paths to the data files, and many sdrf files are still outdated. You might need to update them in the sdrf file.
