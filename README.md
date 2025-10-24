

## How to Run?



1. Create conda environment using the `flsc.yml` file:
   - `conda env create -f environment.yml`
2. Prepare datasets and add the dataset paths under `data_loader/dataset_paths.json`.
   - The dataset paths should be in the following format:
     ```
     {
        "dataset_name": {"train": "path/to/train/dataset",
                         "test": "path/to/test/dataset"},
        ...
     }
     ```
3. For main (accuracy) experiments, run the `main.py` script:
   - `python main.py {desired experiment settings}`
   - Refer to `arg_parser.py` for the list of available arguments.

4. For the experiments involving communication and computation, run the `comm_main.py` script:
   - `python comm_main.py {desired experiment settings}`
   - Refer to `comm_arg_parser.py` for the list of available arguments.


