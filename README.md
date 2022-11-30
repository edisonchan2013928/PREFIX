# PREFIX (Code Descriptions)
This code is the implementation of our paper "PREFIX: A Theoretically Improved Solution for Spatial-Temporal Kernel Density Visualization", which is submitted to PVLDB 2023. Due to space limitations of the Github repository, we do not upload the datasets into this link. However, all datasets are the open data, which can be downloaded from the references in Table 3 (cf. the column "Ref."). The shell script file "compile_run.sh" includes the details for compiling and running our C++ code. We have also attached "exanple_data_file" to show the data format of the input data file.

The file "otf_visual.cpp" shows the implementation of the methods, SWS (lines 37 to 63) and PREFIX<sub>single</sub> (lines 90 to 124), for generating STKDV (cf. Problem 1) with on-the-fly timestamps.

The file "kt_visual.cpp" shows the implementation of the methods, SWS (lines 136 to 145) and PREFIX<sub>multiple</sub> (lines 47 to 134), for generating STKDV (cf. Problem 1) with T known timestamps.

The file "bt_visual.cpp" shows the implementation of the methods, SWS (lines 216 to 239) and PREFIX<sub>tuning</sub> (lines 118 to 214), for bandwidth tuning (cf. Problem 2).

# PREFIX (Technical Report)
Due to space limitations of PVLDB, we do not provide a detailed proof of Lemma 1 in the paper. In this Github link, we also include the technical report (PREFIX_TR.pdf), which shows the proof in Section 7. Since the letters and figures are deformed when we view the pdf file in the anonymized Github link, you can first download this file and then read it in your local computer.
