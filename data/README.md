# Dataset for TGBully

Our experiments use two public datasets crawled from Instagram and Vine.
The datasets were respectively introduced and released in [1] and [2]. 
Please reach out to the wonderful [CU Boulder team](https://sites.google.com/site/cucybersafety/home/cyberbullying-detection-project/dataset) for the datasets.

The CU Boulder team provides 3 csv files for the Instagram dataset -- `sessions_0plus_to_10_metadata.csv`, `sessions_10plus_to_40_metadata.csv`, and `sessions_40plus_metadata.csv`.

The CU Boulder team also provide the user "follows" and "followed" list in files `Instagram_common_users.zip` and `Instagram_normal_users.zip`.
Extract the network statistics and detailed network into the following 2 files, and place them in the `data/ins/` folder.

Similarly, extract the session data `vine_labeled_cyberbullying_data.csv` from the Vine dataset, and place them in the `data/vine/` folder. 

We use [word2vec-twitter](https://github.com/loretoparisi/word2vec-twitter) for word embeddings.
We also provide an off-the-shelf pickle version in the follwing url:
'https://drive.google.com/file/d/1PqHeFg8QvXX_vGv54kgjRZK89XO6Gde0/view?usp=sharing', 'https://drive.google.com/file/d/1onEQw6yFAslUNlZeuviWp6_UyVyoB3KM/view?usp=sharing',
download them and place their path as `w2vVocab_file` and `w2vVector_file` respectively.

### Reference
> \[1\] Homa Hosseinmardi, Sabrina Arredondo Mattson, Rahat Ibn Rafiq, Richard Han, Qin Lv, and Shivakant Mishra. 2015. Analyzing labeled cyberbullying incidents on the instagram social network. In Socinfo. Springer, 49–66.
> 
> \[2\] Rahat Ibn Rafiq, Homa Hosseinmardi, Richard Han, Qin Lv, Shivakant Mishra, and Sabrina Arredondo Mattson. 2015. Careful what you share in six seconds: Detecting cyberbullying instances in Vine. In ASONAM. ACM, 617–622.