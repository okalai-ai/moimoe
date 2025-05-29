
# Noun Class Recognition (NCR) Dataset: WikiNCR

This dataset contains Noun Class Recognition (NCR) in various Bantu languages. It is organized by language, and within each language directory, you’ll find the relevant data files for training, validation, and testing.

----

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

- Xhosa
- Zulu
- Swahili


##  Noun Class Distributions

For each language, a bar chart summarizing the frequency of noun classes (labels) across all data splits (`train`, `val`, and `test`) is provided.

These plots can be found in the `_plots/` directory, each saved as a `.png` file named:
<LANGUAGE>_label_distribution.png

### Example:
- `plots/ZULU_label_distribution.png` shows the frequency of noun class labels for Zulu.

Each chart has:
- The noun class labels on the x-axis
- The number of nouns in each class on the y-axis

These plots are useful for:
- Understanding the class balance
- Spotting overrepresented or rare noun classes
- Informing data augmentation or sampling strategies


##  Noun Class Distribution Table (HTML)

An aggregated HTML table is also available, summarizing the noun class frequencies for each language in a single view.

-  Location: `_plots/noun_class_distribution_table_WikiNCR.html`

### Table Format:
- Rows represent noun classes (e.g., `1`, `2`, `9a`, `14`, etc.)
- Columns represent languages (e.g., `SWAHILI`, `XHOSA`, `ZULU`)
- Each cell shows the number of occurrences of that noun class in the corresponding language.

This table is helpful for:
- Direct cross-language comparison
- Visualizing the overall noun class coverage and balance
- Identifying gaps or skews in annotation per language