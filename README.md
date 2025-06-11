# bert_base_vn_deploy

## HOW TO RUN

Step 1: Clone the repository

Step 2: Create venv with `Python3.10`

```bash
python3.10 -m venv myenv
```

Step 3: Activate the virtual environment

Linux:

```bash
source myenv/bin/activate
```

Windows:

```bash
.\myenv\Scripts\activate
```

Step 4: Install the required packages

```bash
pip install -r requirements.txt
```

Step 5: Run the application

- For files that contain splitted sentences, run:

```bash
python align_sents.py <path_to_chinese_snts_file> <path_to_vietnamese_snts_file> <path_to_output_file>
```

- For files that contain paragraphs, run:

```bash
python align_pars.py <path_to_chinese_paragraphs_file> <path_to_vietnamese_paragraphs_file> <path_to_output_file>
```

- For files that does not belong to the above two cases, run:

```bash
python align_other.py <path_to_chinese_file> <path_to_vietnamese_file> <path_to_output_file>
```
