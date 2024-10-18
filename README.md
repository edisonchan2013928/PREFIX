# Code Descriptions
This code is the implementation of our paper "Large-scale Spatiotemporal Kernel Density Visualization", which is submitted to ICDE 2025. Due to space limitations of the Github repository, we do not upload the datasets into this link. However, all datasets are the open data, which can be downloaded from the references in Table III (see the column "Ref."). We have also attached "[example_data_file](example_data_file)" to show the format of the input data file.

The file "[otf_visual.cpp](otf_visual.cpp)" shows the implementation of the methods, SWS (lines 37 to 63) and PREFIX<sub>single</sub> (lines 90 to 124), for generating STKDV (see Problem 1) with on-the-fly timestamps.

The file "[kt_visual.cpp](kt_visual.cpp)" shows the implementation of the methods, SWS (lines 136 to 145) and PREFIX<sub>multiple</sub> (lines 47 to 134), for generating STKDV (see Problem 1) with T known timestamps.

The file "[bt_visual.cpp](bt_visual.cpp)" shows the implementation of the methods, SWS (lines 216 to 239) and PREFIX<sub>tuning</sub> (lines 118 to 214), for bandwidth tuning (see Problem 2).

# How to Call Our Code?
In order to compile our C++ code, you need to write the following shell scripts in the ".sh file".
```
g++ -c init_visual.cpp -o init_visual.o
g++ -c Euclid_Bound.cpp -o Euclid_Bound.o
g++ -c SS.cpp -o SS.o
g++ -c SWS.cpp -o SWS.o
g++ -c bucket.cpp -o bucket.o
g++ -c otf_visual.cpp -o otf_visual.o
g++ -c kt_visual.cpp -o kt_visual.o
g++ -c bt_visual.cpp -o bt_visual.o
g++ -c alg_visual.cpp -o alg_visual.o
g++ main.cpp -O3 -o main init_visual.o Euclid_Bound.o SS.o SWS.o bucket.o otf_visual.o kt_visual.o bt_visual.o alg_visual.o
```

After you have successfully compiled our C++ code, you can run our C++ code by inputting the correct parameters. Here, we discuss the details about the input parameters in our C++ code.

<!--- The shell script file "[compile_run.sh](compile_run.sh)" includes the details for compiling and running our C++ code.--->


<!--- # PREFIX (Technical Report)
Due to space limitations of PVLDB, we do not provide a detailed proof of Lemma 1 in the paper. In this Github link, we also include the technical report ([PREFIX_TR.pdf](PREFIX_TR.pdf)), which shows the proof in Section 7. Since the letters and figures are deformed when you view the pdf file in the anonymized Github link, you can first download this file and then read it in your local computer.--->
