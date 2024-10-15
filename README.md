# automl-conda-yml-debugg

### Dependency Mismatches 

- nothing provides libcublas >=12.1.0.26,<12.1.3.1 needed by pytorch-cuda-12.1-ha16c6d3_5
 
- nothing provides cuda-cudart >=11.8,<12.0 needed by pytorch-cuda-11.8-h7e8668a_3

- blas 2.16**  is installable with the potential options

- libuuid 2.38.1**  is requested and can be installed;

- llvm-openmp 15.0.7**  is requested and can be installed;

- mkl 2020.2**  is requested and can be installed;

- numpy 1.23.5**  is installable with the potential options

- python 3.9.19**  is not installable because it conflicts with any installable versions previously reported;

- python_abi 3.9**  is installable with the potential options

- pytorch-cuda 12.1**  is not installable because it requires

- pytorch 2.2.2**  is installable with the potential options

<details>
  <summary>error message</summary>
  <br>
  
```
======Starting Image Build on Serverless Compute======
The run ID for the image build on serverless compute is imgbldrun_7cd3461
Additional logs for the run: https://ml.azure.com/experiments/id/prepare_image/runs/imgbldrun_7cd3461?wsid=/subscriptions/e6b2576a-d64f-4ef2-a429-ec3fde2a21db/resourcegroups/inbrein-azure-ml-research/workspaces/inbrein-azure-ml-research-eunsang&tid=5e0527d0-b0a8-46e9-b753-db3f51fb4dc2
2024-10-15T00:33:45: Logging into Docker registry: eunsangacr.azurecr.io
2024-10-15T00:33:45: WARNING! Using --password via the CLI is insecure. Use --password-stdin.
2024-10-15T00:33:45: WARNING! Your password will be stored unencrypted in /root/.docker/config.json.
2024-10-15T00:33:45: Configure a credential helper to remove this warning. See
2024-10-15T00:33:45: https://docs.docker.com/engine/reference/commandline/login/#credentials-store

2024-10-15T00:33:45: Login Succeeded


2024-10-15T00:33:45: Running: ['docker', 'build', '-f', 'azureml-environment-setup/Dockerfile', '.', '-t', 'eunsangacr.azurecr.io/azureml/azureml_c248495abd8eaaa562bfe1fd02341bdd', '-t', 'eunsangacr.azurecr.io/azureml/azureml_c248495abd8eaaa562bfe1fd02341bdd:1']
2024-10-15T00:33:45: DEPRECATED: The legacy builder is deprecated and will be removed in a future release.
2024-10-15T00:33:45:             Install the buildx component to build images with BuildKit:
2024-10-15T00:33:45:             https://docs.docker.com/go/buildx/

2024-10-15T00:33:45: Sending build context to Docker daemon  77.31kB
2024-10-15T00:33:45: Step 1/17 : FROM mcr.microsoft.com/azureml/openmpi4.1.0-ubuntu20.04:latest@sha256:be42e92cad29c2691a55549e982338ce545d29cd61f782ef9c002beaf30a6568
2024-10-15T00:33:45: mcr.microsoft.com/azureml/openmpi4.1.0-ubuntu20.04:latest@sha256:be42e92cad29c2691a55549e982338ce545d29cd61f782ef9c002beaf30a6568: Pulling from azureml/openmpi4.1.0-ubuntu20.04
2024-10-15T00:33:45: 560c024910be: Pulling fs layer
2024-10-15T00:33:45: 46e89cb70915: Pulling fs layer
2024-10-15T00:33:45: fe7e11aee5ca: Pulling fs layer
2024-10-15T00:33:45: 723a8dc12fe7: Pulling fs layer
2024-10-15T00:33:45: cce13f070624: Pulling fs layer
2024-10-15T00:33:45: 27e5996e07ff: Pulling fs layer
2024-10-15T00:33:45: 0f08c6749977: Pulling fs layer
2024-10-15T00:33:45: c2eb857e4a51: Pulling fs layer
2024-10-15T00:33:45: 2a959ffc01ef: Pulling fs layer
2024-10-15T00:33:45: 6b8d3d559c94: Pulling fs layer
2024-10-15T00:33:45: 723a8dc12fe7: Waiting
2024-10-15T00:33:45: cce13f070624: Waiting
2024-10-15T00:33:45: 27e5996e07ff: Waiting
2024-10-15T00:33:45: 0f08c6749977: Waiting
2024-10-15T00:33:45: c2eb857e4a51: Waiting
2024-10-15T00:33:45: 2a959ffc01ef: Waiting
2024-10-15T00:33:45: 6b8d3d559c94: Waiting
2024-10-15T00:33:45: fe7e11aee5ca: Verifying Checksum
2024-10-15T00:33:45: fe7e11aee5ca: Download complete
2024-10-15T00:33:45: 723a8dc12fe7: Verifying Checksum
2024-10-15T00:33:45: 723a8dc12fe7: Download complete
2024-10-15T00:33:45: 560c024910be: Verifying Checksum
2024-10-15T00:33:45: 560c024910be: Download complete
2024-10-15T00:33:45: cce13f070624: Verifying Checksum
2024-10-15T00:33:45: cce13f070624: Download complete
2024-10-15T00:33:45: 0f08c6749977: Verifying Checksum
2024-10-15T00:33:45: 0f08c6749977: Download complete
2024-10-15T00:33:46: c2eb857e4a51: Verifying Checksum
2024-10-15T00:33:46: c2eb857e4a51: Download complete
2024-10-15T00:33:46: 27e5996e07ff: Verifying Checksum
2024-10-15T00:33:46: 27e5996e07ff: Download complete
2024-10-15T00:33:46: 46e89cb70915: Verifying Checksum
2024-10-15T00:33:46: 46e89cb70915: Download complete
2024-10-15T00:33:46: 2a959ffc01ef: Verifying Checksum
2024-10-15T00:33:46: 2a959ffc01ef: Download complete
2024-10-15T00:33:46: 6b8d3d559c94: Verifying Checksum
2024-10-15T00:33:46: 6b8d3d559c94: Download complete
2024-10-15T00:33:47: 560c024910be: Pull complete
2024-10-15T00:33:56: 46e89cb70915: Pull complete
2024-10-15T00:33:57: fe7e11aee5ca: Pull complete
2024-10-15T00:33:57: 723a8dc12fe7: Pull complete
2024-10-15T00:33:57: cce13f070624: Pull complete
2024-10-15T00:34:02: 27e5996e07ff: Pull complete
2024-10-15T00:34:03: 0f08c6749977: Pull complete
2024-10-15T00:34:04: c2eb857e4a51: Pull complete
2024-10-15T00:34:04: 2a959ffc01ef: Pull complete
2024-10-15T00:34:04: 6b8d3d559c94: Pull complete
2024-10-15T00:34:04: Digest: sha256:be42e92cad29c2691a55549e982338ce545d29cd61f782ef9c002beaf30a6568
2024-10-15T00:34:04: Status: Downloaded newer image for mcr.microsoft.com/azureml/openmpi4.1.0-ubuntu20.04:latest@sha256:be42e92cad29c2691a55549e982338ce545d29cd61f782ef9c002beaf30a6568
2024-10-15T00:34:04:  ---> 005da6fe2f84
2024-10-15T00:34:04: Step 2/17 : USER root
2024-10-15T00:34:04:  ---> Running in 52feb335c20d
2024-10-15T00:34:05: Removing intermediate container 52feb335c20d
2024-10-15T00:34:05:  ---> a6d087ca93d5
2024-10-15T00:34:05: Step 3/17 : RUN mkdir -p $HOME/.cache
2024-10-15T00:34:05:  ---> Running in 12dbbf3be61d
2024-10-15T00:34:07: Removing intermediate container 12dbbf3be61d
2024-10-15T00:34:07:  ---> ce41eecf38be
2024-10-15T00:34:07: Step 4/17 : WORKDIR /
2024-10-15T00:34:07:  ---> Running in 1c32b9e4b1d5
2024-10-15T00:34:08: Removing intermediate container 1c32b9e4b1d5
2024-10-15T00:34:08:  ---> 7fa7a2ab1748
2024-10-15T00:34:08: Step 5/17 : COPY azureml-environment-setup/99brokenproxy /etc/apt/apt.conf.d/
2024-10-15T00:34:09:  ---> 780b59b8c9fe
2024-10-15T00:34:09: Step 6/17 : RUN if dpkg --compare-versions `conda --version | grep -oE '[^ ]+$'` lt 4.4.11; then conda install conda==4.4.11; fi
2024-10-15T00:34:09:  ---> Running in 5335511e34bf
2024-10-15T00:34:12: Removing intermediate container 5335511e34bf
2024-10-15T00:34:12:  ---> 5fc565f85750
2024-10-15T00:34:12: Step 7/17 : COPY azureml-environment-setup/mutated_conda_dependencies.yml azureml-environment-setup/mutated_conda_dependencies.yml
2024-10-15T00:34:13:  ---> 94833793e551
2024-10-15T00:34:13: Step 8/17 : RUN ldconfig /usr/local/cuda/lib64/stubs && conda env create -p /azureml-envs/azureml_dd96900caaa7a5e53cd8e1ee04196ebd -f azureml-environment-setup/mutated_conda_dependencies.yml && rm -rf "$HOME/.cache/pip" && conda clean -aqy && CONDA_ROOT_DIR=$(conda info --root) && rm -rf "$CONDA_ROOT_DIR/pkgs" && find "$CONDA_ROOT_DIR" -type d -name __pycache__ -exec rm -rf {} + && ldconfig
2024-10-15T00:34:13:  ---> Running in 674282cdb28c
2024-10-15T00:34:14: Retrieving notices: ...working... done
2024-10-15T00:34:14: Channels:
2024-10-15T00:34:14:  - conda-forge
2024-10-15T00:34:14:  - anaconda
2024-10-15T00:34:14:  - pytorch
2024-10-15T00:34:14:  - defaults
2024-10-15T00:34:14: Platform: linux-64
2024-10-15T00:34:33: Collecting package metadata (repodata.json): ...working... done
2024-10-15T00:36:04: Solving environment: ...working... failed
2024-10-15T00:36:04: Channels:
2024-10-15T00:36:04:  - conda-forge
2024-10-15T00:36:04:  - anaconda
2024-10-15T00:36:04:  - pytorch
2024-10-15T00:36:04:  - defaults
2024-10-15T00:36:04: Platform: linux-64
2024-10-15T00:36:07: Collecting package metadata (repodata.json): ...working... done
2024-10-15T00:37:41: Solving environment: ...working... failed
2024-10-15T00:37:41: [91m
2024-10-15T00:37:41: LibMambaUnsatisfiableError: Encountered problems while solving:
2024-10-15T00:37:41:   - nothing provides libcublas >=12.1.0.26,<12.1.3.1 needed by pytorch-cuda-12.1-ha16c6d3_5
2024-10-15T00:37:41:   - nothing provides cuda-cudart >=11.8,<12.0 needed by pytorch-cuda-11.8-h7e8668a_3

2024-10-15T00:37:41: Could not solve for environment specs
2024-10-15T00:37:41: The following packages are incompatible
2024-10-15T00:37:41: ├─ blas 2.16**  is installable with the potential options
2024-10-15T00:37:41: │  ├─ blas 2.16 would require
2024-10-15T00:37:41: │  │  └─ liblapacke 3.8.0 16_mkl, which requires
2024-10-15T00:37:41: │  │     ├─ blas * mkl, which can be installed;
2024-10-15T00:37:41: │  │     └─ libblas 3.8.0 16_mkl, which requires
2024-10-15T00:37:41: │  │        └─ liblapack 3.8.0 16_mkl, which can be installed;
2024-10-15T00:37:41: │  ├─ blas 2.16 conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  └─ blas [2.10|2.11|...|2.9] would require
2024-10-15T00:37:41: │     └─ liblapacke [3.8.0 10_openblas|3.8.0 11_openblas|...|3.8.0 9_openblas] but there are no viable options
2024-10-15T00:37:41: │        ├─ liblapacke 3.8.0 would require
2024-10-15T00:37:41: │        │  └─ blas * openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        └─ liblapacke 3.8.0 would require
2024-10-15T00:37:41: │           └─ blas * openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: ├─ libuuid 2.38.1**  is requested and can be installed;
2024-10-15T00:37:41: ├─ llvm-openmp 15.0.7**  is requested and can be installed;
2024-10-15T00:37:41: ├─ mkl 2020.2**  is requested and can be installed;
2024-10-15T00:37:41: ├─ numpy 1.23.5**  is installable with the potential options
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python_abi 3.10.* *_cp310, which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python_abi 3.11.* *_cp311, which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python_abi 3.8.* *_cp38, which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python_abi 3.8 *_pypy38_pp73, which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ liblapack >=3.9.0,<4.0a0  but there are no viable options
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 0_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas [3.9.0 10_mkl|3.9.0 11_linux64_mkl], which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2021.3.0,<2022.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 10_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 11_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas 3.9.0 12_linux64_mkl, which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2021.4.0,<2022.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 12_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas [3.9.0 13_linux64_mkl|3.9.0 14_linux64_mkl], which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2022.0.1,<2023.0a0  but there are no viable options
2024-10-15T00:37:41: │  │     │        ├─ mkl [2022.2.1|2024.2.0|2024.2.1|2024.2.2] would require
2024-10-15T00:37:41: │  │     │        │  └─ llvm-openmp >=18.1.8 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        ├─ mkl 2022.0.1 conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        └─ mkl [2022.1.0|2022.2.1] conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 13_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 14_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas [3.9.0 15_linux64_mkl|3.9.0 16_linux64_mkl], which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2022.1.0,<2023.0a0  but there are no viable options
2024-10-15T00:37:41: │  │     │        ├─ mkl [2022.2.1|2024.2.0|2024.2.1|2024.2.2], which cannot be installed (as previously explained);
2024-10-15T00:37:41: │  │     │        └─ mkl [2022.1.0|2022.2.1] conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 15_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 16_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 1_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 2_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 3_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas [3.9.0 4_mkl|3.9.0 5_mkl|3.9.0 6_mkl|3.9.0 7_mkl|3.9.0 8_mkl], which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2020.4,<2021.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 4_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 5_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 6_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 7_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 8_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas 3.9.0 9_mkl, which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2021.2.0,<2022.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 9_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 17_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 18_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas [3.9.0 19_linux64_mkl|3.9.0 20_linux64_mkl], which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2023.2.0,<2024.0a0  but there are no viable options
2024-10-15T00:37:41: │  │     │        ├─ mkl 2023.2.0 would require
2024-10-15T00:37:41: │  │     │        │  └─ llvm-openmp >=16.0.6 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        └─ mkl 2023.2.0 would require
2024-10-15T00:37:41: │  │     │           └─ llvm-openmp >=17.0.3 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 19_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 20_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas 3.9.0 21_linux64_mkl, which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2024.0.0,<2025.0a0  but there are no viable options
2024-10-15T00:37:41: │  │     │        ├─ mkl 2024.0.0 would require
2024-10-15T00:37:41: │  │     │        │  └─ llvm-openmp >=17.0.6 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        ├─ mkl 2024.1.0 would require
2024-10-15T00:37:41: │  │     │        │  └─ llvm-openmp >=18.1.2 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        ├─ mkl 2024.1.0 would require
2024-10-15T00:37:41: │  │     │        │  └─ llvm-openmp >=18.1.3 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        ├─ mkl 2024.1.0 would require
2024-10-15T00:37:41: │  │     │        │  └─ llvm-openmp >=18.1.5 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     │        └─ mkl [2022.2.1|2024.2.0|2024.2.1|2024.2.2], which cannot be installed (as previously explained);
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 21_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ libblas [3.9.0 22_linux64_mkl|3.9.0 23_linux64_mkl|3.9.0 24_linux64_mkl], which requires
2024-10-15T00:37:41: │  │     │     └─ mkl >=2024.1.0,<2025.0a0 , which cannot be installed (as previously explained);
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 22_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │     │  └─ liblapacke 3.9.0 23_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     └─ liblapack 3.9.0 would require
2024-10-15T00:37:41: │  │        └─ liblapacke 3.9.0 24_linux64_openblas, which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python_abi 3.9 *_pypy39_pp73, which requires
2024-10-15T00:37:41: │  │     └─ python 3.9.* *_73_pypy, which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python >=3.10,<3.11.0a0  with the potential options
2024-10-15T00:37:41: │  │     ├─ python [3.10.0|3.10.1|...|3.10.9] would require
2024-10-15T00:37:41: │  │     │  └─ python_abi 3.10.* *_cp310, which can be installed;
2024-10-15T00:37:41: │  │     ├─ python 3.10.8 would require
2024-10-15T00:37:41: │  │     │  └─ python_abi 3.10.* *_graalpy230_310_native, which can be installed;
2024-10-15T00:37:41: │  │     ├─ python [3.10.0|3.10.3|3.10.4|3.10.6|3.10.8] would require
2024-10-15T00:37:41: │  │     │  └─ libuuid >=1.0.3,<2.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     └─ python [3.10.10|3.10.11|...|3.12.7] would require
2024-10-15T00:37:41: │  │        └─ libuuid >=1.41.5,<2.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python >=3.11,<3.12.0a0  with the potential options
2024-10-15T00:37:41: │  │     ├─ python [3.10.10|3.10.11|...|3.12.7], which cannot be installed (as previously explained);
2024-10-15T00:37:41: │  │     └─ python [3.11.0|3.11.1|...|3.11.9] would require
2024-10-15T00:37:41: │  │        └─ python_abi 3.11.* *_cp311, which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ python >=3.8,<3.9.0a0  with the potential options
2024-10-15T00:37:41: │  │     ├─ python [3.8.0|3.8.1] would require
2024-10-15T00:37:41: │  │     │  └─ python_abi * *_cp38, which can be installed;
2024-10-15T00:37:41: │  │     ├─ python [3.8.10|3.8.12|...|3.8.8] would require
2024-10-15T00:37:41: │  │     │  └─ python_abi 3.8.* *_cp38, which can be installed;
2024-10-15T00:37:41: │  │     ├─ python [3.8.12|3.8.13|3.8.16] would require
2024-10-15T00:37:41: │  │     │  └─ python_abi 3.8 *_pypy38_pp73, which can be installed;
2024-10-15T00:37:41: │  │     ├─ python 3.8.5 would require
2024-10-15T00:37:41: │  │     │  └─ python_abi 3.8.* *_graalpy223_38_native, which can be installed;
2024-10-15T00:37:41: │  │     └─ python [3.8.0|3.8.1|...|3.8.8], which can be installed;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ mkl >=2021.4.0,<2022.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  ├─ numpy 1.23.5 would require
2024-10-15T00:37:41: │  │  └─ mkl >=2023.1.0,<2024.0a0  but there are no viable options
2024-10-15T00:37:41: │  │     ├─ mkl 2023.1.0 would require
2024-10-15T00:37:41: │  │     │  └─ llvm-openmp >=16.0.1 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  │     ├─ mkl 2023.2.0, which cannot be installed (as previously explained);
2024-10-15T00:37:41: │  │     ├─ mkl 2023.2.0, which cannot be installed (as previously explained);
2024-10-15T00:37:41: │  │     └─ mkl 2023.1.0 conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  └─ numpy 1.23.5 would require
2024-10-15T00:37:41: │     └─ blas * openblas but there are no viable options
2024-10-15T00:37:41: │        ├─ blas 2.119 would require
2024-10-15T00:37:41: │        │  └─ llvm-openmp >=17.0.2 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        ├─ blas 2.120 would require
2024-10-15T00:37:41: │        │  └─ llvm-openmp >=17.0.5 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        ├─ blas 2.121 would require
2024-10-15T00:37:41: │        │  └─ llvm-openmp >=17.0.6 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        ├─ blas 2.122 would require
2024-10-15T00:37:41: │        │  └─ llvm-openmp >=18.1.2 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        ├─ blas [2.123|2.124] would require
2024-10-15T00:37:41: │        │  └─ llvm-openmp >=18.1.8 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        ├─ blas [2.10|2.11|...|2.9], which cannot be installed (as previously explained);
2024-10-15T00:37:41: │        ├─ blas [1.0|1.1|...|2.3] conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        ├─ blas [2.4|2.5|2.6|2.7] would require
2024-10-15T00:37:41: │        │  └─ libblas [3.8.0 4_openblas|3.8.0 5_openblas|3.8.0 6_openblas|3.8.0 7_openblas], which requires
2024-10-15T00:37:41: │        │     └─ openblas 0.3.5.* , which does not exist (perhaps a missing channel);
2024-10-15T00:37:41: │        ├─ blas 2.117 would require
2024-10-15T00:37:41: │        │  └─ llvm-openmp >=16.0.5 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │        └─ blas 2.118 would require
2024-10-15T00:37:41: │           └─ llvm-openmp >=16.0.6 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41: ├─ python 3.9.19**  is not installable because it conflicts with any installable versions previously reported;
2024-10-15T00:37:41: ├─ python_abi 3.9**  is installable with the potential options
2024-10-15T00:37:41: │  ├─ python_abi 3.9 conflicts with any installable versions previously reported;
2024-10-15T00:37:41: │  └─ python_abi 3.9, which can be installed (as previously explained);
2024-10-15T00:37:41: ├─ pytorch-cuda 12.1**  is not installable because it requires
2024-10-15T00:37:41: │  └─ libcublas >=12.1.0.26,<12.1.3.1 , which does not exist (perhaps a missing channel);
2024-10-15T00:37:41: └─ pytorch 2.2.2**  is installable with the potential options
2024-10-15T00:37:41:    ├─ pytorch 2.2.2 would require
2024-10-15T00:37:41:    │  └─ python >=3.8,<3.9.0a0  with the potential options
2024-10-15T00:37:41:    │     ├─ python [3.8.0|3.8.1], which can be installed (as previously explained);
2024-10-15T00:37:41:    │     ├─ python [3.8.10|3.8.12|...|3.8.8], which can be installed (as previously explained);
2024-10-15T00:37:41:    │     ├─ python [3.8.12|3.8.13|3.8.16], which can be installed (as previously explained);
2024-10-15T00:37:41:    │     ├─ python 3.8.5, which can be installed (as previously explained);
2024-10-15T00:37:41:    │     └─ python [3.8.0|3.8.1|...|3.8.8], which can be installed;
2024-10-15T00:37:41:    ├─ pytorch 2.2.2 would require
2024-10-15T00:37:41:    │  └─ python >=3.10,<3.11.0a0  with the potential options
2024-10-15T00:37:41:    │     ├─ python [3.10.0|3.10.1|...|3.10.9], which can be installed (as previously explained);
2024-10-15T00:37:41:    │     ├─ python 3.10.8, which can be installed (as previously explained);
2024-10-15T00:37:41:    │     ├─ python [3.10.0|3.10.3|3.10.4|3.10.6|3.10.8], which cannot be installed (as previously explained);
2024-10-15T00:37:41:    │     └─ python [3.10.10|3.10.11|...|3.12.7], which cannot be installed (as previously explained);
2024-10-15T00:37:41:    ├─ pytorch 2.2.2 would require
2024-10-15T00:37:41:    │  └─ pytorch-cuda >=11.8,<11.9  but there are no viable options
2024-10-15T00:37:41:    │     ├─ pytorch-cuda 11.8 would require
2024-10-15T00:37:41:    │     │  └─ cuda-cudart >=11.8,<12.0 , which does not exist (perhaps a missing channel);
2024-10-15T00:37:41:    │     └─ pytorch-cuda 11.8 would require
2024-10-15T00:37:41:    │        └─ cuda 11.8.* , which does not exist (perhaps a missing channel);
2024-10-15T00:37:41:    ├─ pytorch 2.2.2 would require
2024-10-15T00:37:41:    │  └─ pytorch-cuda >=12.1,<12.2 , which cannot be installed (as previously explained);
2024-10-15T00:37:41:    ├─ pytorch 2.2.2 would require
2024-10-15T00:37:41:    │  └─ python >=3.11,<3.12.0a0  with the potential options
2024-10-15T00:37:41:    │     ├─ python [3.10.10|3.10.11|...|3.12.7], which cannot be installed (as previously explained);
2024-10-15T00:37:41:    │     └─ python [3.11.0|3.11.1|...|3.11.9], which can be installed (as previously explained);
2024-10-15T00:37:41:    ├─ pytorch 2.2.2 would require
2024-10-15T00:37:41:    │  └─ python >=3.12,<3.13.0a0  with the potential options
2024-10-15T00:37:41:    │     ├─ python [3.10.10|3.10.11|...|3.12.7], which cannot be installed (as previously explained);
2024-10-15T00:37:41:    │     └─ python [3.12.0|3.12.1|...|3.12.7] would require
2024-10-15T00:37:41:    │        └─ python_abi 3.12.* *_cp312, which can be installed;
2024-10-15T00:37:41:    └─ pytorch 2.2.2 would require
2024-10-15T00:37:41:       └─ blas * mkl with the potential options
2024-10-15T00:37:41:          ├─ blas [1.0|2.15], which can be installed;
2024-10-15T00:37:41:          ├─ blas [2.10|2.11|...|2.9] would require
2024-10-15T00:37:41:          │  └─ libblas [3.8.0 10_mkl|3.8.0 11_mkl|...|3.8.0 9_mkl], which requires
2024-10-15T00:37:41:          │     └─ mkl >=2019.0,<2020.0a0 , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41:          ├─ blas [2.105|2.106|2.107|2.108] would require
2024-10-15T00:37:41:          │  └─ libblas [3.9.0 5_mkl|3.9.0 6_mkl|3.9.0 7_mkl|3.9.0 8_mkl], which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas 2.109 would require
2024-10-15T00:37:41:          │  └─ libblas 3.9.0 9_mkl, which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas [2.110|2.111] would require
2024-10-15T00:37:41:          │  └─ libblas [3.9.0 10_mkl|3.9.0 11_linux64_mkl], which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas 2.112 would require
2024-10-15T00:37:41:          │  └─ libblas 3.9.0 12_linux64_mkl, which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas [2.113|2.114] would require
2024-10-15T00:37:41:          │  └─ libblas [3.9.0 13_linux64_mkl|3.9.0 14_linux64_mkl], which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas [2.115|2.116] would require
2024-10-15T00:37:41:          │  └─ libblas [3.9.0 15_linux64_mkl|3.9.0 16_linux64_mkl], which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas 2.16, which can be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas [2.18|2.19|2.20|2.21] would require
2024-10-15T00:37:41:          │  └─ liblapacke [3.8.0 18_mkl|3.8.0 19_mkl|3.8.0 20_mkl|3.8.0 21_mkl], which requires
2024-10-15T00:37:41:          │     └─ blas * mkl, which can be installed;
2024-10-15T00:37:41:          ├─ blas 2.4 would require
2024-10-15T00:37:41:          │  └─ libblas 3.8.0 4_mkl, which requires
2024-10-15T00:37:41:          │     └─ mkl 2019.1.* , which conflicts with any installable versions previously reported;
2024-10-15T00:37:41:          ├─ blas 2.119, which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas 2.120, which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas 2.121, which cannot be installed (as previously explained);
2024-10-15T00:37:41:          ├─ blas 2.122, which cannot be installed (as previously explained);
2024-10-15T00:37:41:          └─ blas [2.123|2.124], which cannot be installed (as previously explained).

2024-10-15T00:37:41: The command '/bin/sh -c ldconfig /usr/local/cuda/lib64/stubs && conda env create -p /azureml-envs/azureml_dd96900caaa7a5e53cd8e1ee04196ebd -f azureml-environment-setup/mutated_conda_dependencies.yml && rm -rf "$HOME/.cache/pip" && conda clean -aqy && CONDA_ROOT_DIR=$(conda info --root) && rm -rf "$CONDA_ROOT_DIR/pkgs" && find "$CONDA_ROOT_DIR" -type d -name __pycache__ -exec rm -rf {} + && ldconfig' returned a non-zero code: 1

2024-10-15T00:37:41: [0m

2024-10-15T00:37:41: CalledProcessError(1, ['docker', 'build', '-f', 'azureml-environment-setup/Dockerfile', '.', '-t', 'eunsangacr.azurecr.io/azureml/azureml_c248495abd8eaaa562bfe1fd02341bdd', '-t', 'eunsangacr.azurecr.io/azureml/azureml_c248495abd8eaaa562bfe1fd02341bdd:1'])

2024-10-15T00:37:41: Building docker image failed with exit code: 1

2024-10-15T00:37:41: Logging out of Docker registry: eunsangacr.azurecr.io
2024-10-15T00:37:41: Removing login credentials for https://index.docker.io/v1/


2024-10-15T00:37:41: Traceback (most recent call last):
  File "/mnt/azureml/cr/j/194f1f78c5414c829e9415c6648e942d/exe/wd/docker_utilities.py", line 152, in _docker_build_or_error
    docker_execute_function(docker_command, build_command, print_command_args=True)
  File "/mnt/azureml/cr/j/194f1f78c5414c829e9415c6648e942d/exe/wd/docker_utilities.py", line 23, in docker_execute_function
    return killable_subprocess.check_call(command_args, *popen_args,
  File "/mnt/azureml/cr/j/194f1f78c5414c829e9415c6648e942d/exe/wd/killable_subprocess.py", line 261, in check_call
    raise subprocess.CalledProcessError(process.returncode, cmd)
subprocess.CalledProcessError: Command '['docker', 'build', '-f', 'azureml-environment-setup/Dockerfile', '.', '-t', 'eunsangacr.azurecr.io/azureml/azureml_c248495abd8eaaa562bfe1fd02341bdd', '-t', 'eunsangacr.azurecr.io/azureml/azureml_c248495abd8eaaa562bfe1fd02341bdd:1']' returned non-zero exit status 1.

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "script.py", line 110, in <module>
    docker_utilities._docker_build_or_error(
  File "/mnt/azureml/cr/j/194f1f78c5414c829e9415c6648e942d/exe/wd/docker_utilities.py", line 156, in _docker_build_or_error
    _write_error_and_exit(error_msg, error_file_path=error_file_path)
  File "/mnt/azureml/cr/j/194f1f78c5414c829e9415c6648e942d/exe/wd/docker_utilities.py", line 217, in _write_error_and_exit
    sys.exit(1)
SystemExit: 1
```

</details>

