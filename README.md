
Resources Introduced in the paper [Typology-Guided Adaptation in Multilingual Models](https://ndapa.us/assets/docs/papers/2025-moi-acl.pdf) at ACL 2025


# 🗂️ Noun Class Recognition (NCR) Datasets 


Each file contains lines in the following pipe-delimited format:
en_word ||| definition ||| language ||| bantu_word ||| label


### Field Descriptions:

| Field        | Description                                                 |
|--------------|-------------------------------------------------------------|
| `en_word`     | The English noun                                            |
| `definition` | The English definition                                       |
| `language`   | The Bantu language of the data entry, in **uppercase** (e.g., `ZULU`) |
| `bantu_word` | The corresponding word in the target Bantu language         |
| `label`      | A label representing the NCR target                         |

---

##  Languages Included

- Shona
- Xhosa
- Zulu
- Swahili
- Ndonga
- Luganda
- Kwanyama
- Umbundu
- Herero
- Sotho

##  Noun Class Distributions

For each language, a bar chart summarizing the frequency of noun classes (labels) across all data splits (`train`, `val`, and `test`) is provided.

These plots can be found in the `_plots/` directory, each saved as a `.png` file named:
<LANGUAGE>_label_distribution.png

### Example:
- `_plots/ZULU_label_distribution.png` shows the frequency of noun class labels for Zulu.

Each chart has:
- The noun class labels on the x-axis
- The number of nouns in each class on the y-axis

These plots are useful for:
- Understanding the class balance
- Spotting overrepresented or rare noun classes
- Informing data augmentation or sampling strategies

## 🧾 Noun Class Distribution Table (HTML)

An aggregated HTML table is also available, summarizing the noun class frequencies for each language in a single view.

- 📄 Location: `_plots/noun_class_distribution_table_DictNCR.html`

### Table Format:
- Rows represent noun classes (e.g., `1`, `2`, `9a`, `14`, etc.)
- Columns represent languages (e.g., `SWAHILI`, `XHOSA`, `ZULU`)
- Each cell shows the number of occurrences of that noun class in the corresponding language.

This table is helpful for:
- Direct cross-language comparison
- Visualizing the overall noun class coverage and balance
- Identifying gaps or skews in annotation per language



## 📚 Citation

If you use this data for academic research, please cite the following [paper] (https://ndapa.us/assets/docs/papers/2025-moi-acl.pdf):

<pre><code>
@inproceedings{nakashole2025acl,
  author    = {Nakashole, Ndapa},
  title     = {Typology-Guided Adaptation in Multilingual Models},
  booktitle = {Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics},
  year      = {2025},
}
</code></pre>

## 📄 License

This project is licensed under the terms of the **MIT License**.  
You are free to use, modify, and distribute this software with proper attribution.

A full copy of the license is available in the [LICENSE.txt](./LICENSE.txt) file.


