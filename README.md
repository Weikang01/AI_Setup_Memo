# AI_Setup_Memo (2023.07)
> **NOTE**: AI changed very quickly these days
- OS:
  - **Ubuntu** if needed
    - download VMWare Workspace
    - an iso for Ubuntu
- GPU acceleration:
  - **NVidia Geforce**
  - **CUDA toolkit** (use the **`nvidia-smi`** command in the command line to check compatible CUDA version!!)
    ```output
    +---------------------------------------------------------------------------------------+
    | NVIDIA-SMI 536.40                 Driver Version: 536.40       CUDA Version: 12.2     |
    |-----------------------------------------+----------------------+----------------------+
    | GPU  Name                     TCC/WDDM  | Bus-Id        Disp.A | Volatile Uncorr. ECC |
    | Fan  Temp   Perf          Pwr:Usage/Cap |         Memory-Usage | GPU-Util  Compute M. |
    |                                         |                      |               MIG M. |
    |=========================================+======================+======================|
    |   0  NVIDIA GeForce RTX 3070 ...  WDDM  | 00000000:01:00.0 Off |                  N/A |
    | N/A   51C    P8              10W / 140W |   4115MiB /  8192MiB |      0%      Default |
    |                                         |                      |                  N/A |
    +-----------------------------------------+----------------------+----------------------+
    
    +---------------------------------------------------------------------------------------+
    | Processes:                                                                            |
    |  GPU   GI   CI        PID   Type   Process name                            GPU Memory |
    |        ID   ID                                                             Usage      |
    |=======================================================================================|
    |    0   N/A  N/A     12368      C   ...0_x64__qbz5n2kfra8p0\python3.11.exe    N/A      |
    |    0   N/A  N/A     17236    C+G   ...inaries\Win64\EpicGamesLauncher.exe    N/A      |
    +---------------------------------------------------------------------------------------+
    ```
    here is a sample output, see there's a **`CUDA Version: 12.2`**, download the corresponding version of CUDA
  - **CUDnn** (unzip and paste folders to the CUDA installation path)
- IDE:
  - PyCharm
- Python/pip/conda
- PyTorch for CUDA (google the actual command to download the correct version of PyTorch for the corresponding CUDA version
- download the `transformers` library
- Jupyter notebook
- `huggingface_hub`
- other kinds of stuff:
  - pandas, scipy, matplotlib, sklearn, datasets
