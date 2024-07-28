# NeoNyx

🌟 **NeoNyx** - An AI-powered ecosystem for personality typing and analysis

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Future Work](#future-work)
5. [Discussion](#discussion)
6. [Acknowledgements](#acknowledgements)
7. [Contact](#contact)

## Project Overview
NeoNyx is an innovative project focused on creating an ecosystem of AI tools for personality typing and analysis. Leveraging a comprehensive dataset of personality profiles from multiple typing systems, NeoNyx aims to provide insights and applications across various domains, including psychology, marketing, HR, data science, and AI development.

## Dataset Description
- The dataset, `combined_data_highest_voted.csv`, contains detailed personality profiles, descriptions, and multiple typing systems for public figures. Special thanks to [personality-database.com](https://www.personality-database.com/) for providing the data and inspiration for this project! We ensured compliance with their `robots.txt` and limited our request rate.

- The dataset is hosted and available here on [Kaggle](https://www.kaggle.com/datasets/abdelkarimbsalah/nyx-2-1) licensed under the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](LICENSE).

- The cloud version of the analysis notebook is also available on Kaggle [here](https://www.kaggle.com/code/abdelkarimbsalah/neonyx/). 

### CSV File Details
| Column          | Description                                                                                       |
|-----------------|---------------------------------------------------------------------------------------------------|
| `id`            | Unique identifier for each entry                                                                  |
| `mbti_profile`  | Name of the public figure                                                                         |
| `wiki_description` | Text description of the individual sourced from Wikipedia                                       |
| `sub_cat_id`    | Sub-category identifier                                                                           |
| `cat_id`        | Category identifier                                                                               |
| `property_id`   | Property identifier                                                                               |
| `total_vote_counts` | Total number of votes received for the entry                                                  |
| `system_1`      | Personality type according to the first system (MBTI)                                             |
| `system_2`      | Personality type according to the second system (Enneagram)                                       |
| `system_3`      | Personality type according to the third system (Socionics)                                        |
| `system_4`      | Personality type according to the fourth system (Alignment)                                       |
| `system_5`      | Personality type according to the fifth system (Instinctual Variant)                              |
| `system_6`      | Personality type according to the sixth system (Tritype)                                          |
| `system_7`      | Personality type according to the seventh system (Temperament)                                    |
| `system_8`      | Personality type according to the eighth system (Attitudinal Psyche)                              |
| `system_9`      | Personality type according to the ninth system (Big 5 - SLOAN)                                    |
| `system_10`     | Personality type according to the tenth system (Hemispheric Personality Typing)                   |
| `system_11`     | Personality type according to the eleventh system (Classic Jungian)                               |

#### Note
- The value "XXXX" in the typing systems columns indicates a missing value.
- Descriptions provide valuable context for each profile, allowing for in-depth analysis and comparison across different personality typing systems.

## Exploratory Data Analysis (EDA)
The `neonyx.ipynb` notebook provides a detailed analysis of the dataset, including data cleaning, preprocessing, TF-IDF analysis, and word cloud generation. The results highlight key insights, such as average word count and most common words for each MBTI type.

You can view the full analysis in the [neonyx.ipynb](neonyx.ipynb) notebook.

## Future Work
The analysis and findings presented in this study open several exciting avenues for future research and development. Here are some potential directions for future work:

1. **Refinement of Text Processing Techniques** ✨:
   - **Enhancing text preprocessing** methods to better handle variations in language, slang, and regional dialects can improve the accuracy of personality analysis.
   - **Incorporating advanced NLP techniques** such as BERT or GPT for a deeper semantic understanding of descriptions.

2. **Expanding the Dataset** 📈:
   - **Mining more data**: We are currently in the process of collecting additional personality descriptions from various sources to expand the size of our dataset.
   - **Including more personality systems** beyond MBTI, such as the Big Five or Enneagram, to create a more comprehensive personality typing model.

3. **Temporal Analysis** ⏳:
   - Investigating how descriptions of personality types **change over time** can provide insights into the evolving nature of personality traits and societal perceptions.
   - Analyzing the impact of **major events or cultural shifts** on the language used to describe personality types.

4. **Contextual Analysis** 🌐:
   - Exploring how different contexts (e.g., professional, social, academic) influence the language and traits associated with personality types.
   - Developing **context-specific personality typing models** to enhance the relevance and accuracy of predictions.

5. **Applications in AI and Personalization** 🤖:
   - Integrating the findings into **AI-driven applications** for personalized content recommendations, career counselling, and mental health support.
   - Developing more sophisticated personality prediction models that can dynamically adapt to new data and user interactions.

6. **Cross-Cultural Studies** 🌏:
   - Conducting cross-cultural studies to understand how personality descriptions **vary across different cultures and languages**.
   - Adapting personality analysis models to account for **cultural nuances and differences**.


---
---
## Discussion <a name="discussion"></a>

The exploration of the MBTI dataset through various analytical techniques has yielded several insights into the distinct language and characteristics associated with each MBTI type. In this section, we will delve deeper into the results, examining the significance of the findings and their implications for understanding personality traits and behaviors.

### Average Word Count for Each MBTI Type

The average word count analysis reveals the verbosity of descriptions associated with each MBTI type. Here are some notable observations:

1. **INTJ (7.97 words)** and **INTP (7.68 words)** have the highest average word counts, indicating that descriptions of individuals with these personality types tend to be more detailed. This aligns with the introspective and analytical nature of these types, who are often described with complex and nuanced language.
   
2. **ESFJ (5.90 words)** and **ISFJ (6.00 words)** have the lowest average word counts, suggesting that descriptions of these personality types are more concise. This could be attributed to their practical and straightforward nature, which might not require as elaborate descriptions.

3. The overall distribution of average word counts suggests that thinking and judging types (T and J) tend to have longer descriptions, possibly reflecting their more structured and detailed-oriented nature. In contrast, feeling and perceiving types (F and P) have relatively shorter descriptions, which may reflect their more spontaneous and flexible nature.

### Top 5 Most Common Words for Each MBTI Type

The analysis of the top 5 most common words for each MBTI type provides a glimpse into the unique traits and interests that characterize different personality types. Here are some detailed insights:

1. **ESFP**: Words like "dancer," "energetic," and "sports" highlight the outgoing, energetic, and active nature of ESFPs. These individuals are often described as lively and enthusiastic, which is reflected in their common words.

2. **ENTP**: Terms such as "philosopher," "sarcastic," and "animator" emphasize the intellectual and creative traits of ENTPs. They are known for their quick wit and love for debate, which is evident from the language used to describe them.

3. **ENFP**: Words like "cheerful," "energetic," and "dancer" underscore the warm, enthusiastic, and creative nature of ENFPs. Their descriptions reflect their ability to inspire and bring positive energy to social interactions.

4. **ISTJ**: Words such as "soldier," "fought," and "information" indicate the disciplined, reliable, and detail-oriented nature of ISTJs. Their descriptions often emphasize their dedication to duty and precision.

5. **ISFJ**: Common words like "shy," "gentle," and "timid" highlight the nurturing, compassionate, and reserved nature of ISFJs. These individuals are often described in terms that reflect their caring and supportive demeanour.

6. **INTP**: Terms such as "philosopher," "computer," and "theory" emphasize the analytical and abstract thinking traits of INTPs. Their descriptions often focus on their intellectual pursuits and love for theoretical concepts.

7. **ENTJ**: Words like "businessman," "villain," and "ruthless" reflect the assertive, strategic, and ambitious nature of ENTJs. These individuals are often described as natural leaders with a strong drive to achieve their goals.

8. **INTJ**: Common terms such as "genius," "philosopher," and "theory" highlight the intellectual and strategic traits of INTJs. Their descriptions often emphasize their ability to think critically and plan meticulously.

9. **INFP**: Words like "shy," "literature," and "visual" underscore the introspective, creative, and empathetic nature of INFPs. Their descriptions often reflect their deep inner world and love for artistic expression.

10. **INFJ**: Terms such as "philosopher," "prize," and "novelist" emphasize the insightful and idealistic traits of INFJs. Their descriptions often focus on their visionary thinking and deep sense of purpose.

11. **ESTJ**: Words like "attitude," "ruthless," and "lawyer" highlight the practical, decisive, and assertive nature of ESTJs. These individuals are often described as efficient organizers who value structure and order.

12. **ISTP**: Common terms such as "soldier," "mercenary," and "drummer" reflect the adventurous, practical, and resourceful nature of ISTPs. Their descriptions often emphasize their hands-on approach to life.

13. **ISFP**: Words like "dancer," "guitar," and "label" underscore the artistic, sensitive, and spontaneous nature of ISFPs. Their descriptions often reflect their love for creative expression and aesthetics.

14. **ESTP**: Terms such as "businessman," "sports," and "violent" emphasize the energetic, pragmatic, and competitive traits of ESTPs. These individuals are often described as dynamic problem-solvers who thrive in fast-paced environments.

15. **ESFJ**: Words like "cheerful," "presenter," and "sweet" highlight the warm, sociable, and supportive nature of ESFJs. Their descriptions often reflect their ability to create harmony and foster positive relationships.

16. **ENFJ**: Common terms such as "journalist," "cooking," and "entrepreneur" reflect the charismatic, empathetic, and visionary traits of ENFJs. These individuals are often described as inspiring leaders who are dedicated to helping others.

#### Implications and Significance

1. **Personality-Specific Language**: The analysis confirms that different MBTI types are associated with distinct linguistic patterns. This can be leveraged in various applications, such as targeted content creation, personalized marketing, and improved communication strategies.

2. **Enhanced Understanding**: By identifying the common words and average word counts for each MBTI type, we gain a deeper understanding of how different personalities are perceived and described. This can enhance our ability to recognize and appreciate diverse personality traits in social and professional settings.

3. **Applications in AI**: The insights gained from this analysis can be utilized to improve AI models for personality typing and profiling. For instance, incorporating TF-IDF and common word analysis can enhance the accuracy of personality prediction models.

4. **Cultural and Contextual Factors**: The results also highlight the importance of considering cultural and contextual factors in personality descriptions. Words like "dancer" and "sports" may carry different connotations in different cultures, and understanding these nuances is crucial for accurate personality analysis.

5. **Future Research**: Further research can explore the temporal and contextual variations in personality descriptions. For example, analyzing how the language used to describe personalities evolves over time or in different contexts (e.g., social media vs. professional settings) can provide additional valuable insights.

### Conclusion

The exploration of the MBTI dataset through data cleaning, preprocessing, TF-IDF analysis, and word cloud generation has provided valuable insights into the distinct language and characteristics associated with each MBTI type. These findings not only enhance our understanding of personality traits and behaviours but also offer practical applications in fields such as AI, marketing, and communication. Future research can build on these insights to further refine personality analysis and explore new dimensions of personality profiling.

---
---

## Acknowledgements
A special thanks to [personality-database.com](https://www.personality-database.com/) for providing the data and inspiration for this project. We also acknowledge the contributions of the open-source community for their invaluable tools and resources.

## Contact
For any questions, suggestions, or collaborations, feel free to reach out:

- **Email**: [abdelkarimbsalah@gmail.com](mailto:abdelkarimbsalah@gmail.com)
- **LinkedIn**: [Abdelkarim Ben Salah](https://www.linkedin.com/in/abdelkarim-b-salah/)
- **Kaggle**: [abdelkarimbsalah](https://www.kaggle.com/abdelkarimbsalah)

---

📄 **License**: This project is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](LICENSE).
