# Identity Recognition Prompt

## 1. Cantonese and Mandarin Recognition Prompt of LLM

```
You are a language analysis expert. Please determine and output the probabilities of the writer speaking Cantonese and Mandarin, respectively (the probabilities should add up to 100%). Note:
(1) Vocabulary: Cantonese retains more features of Classical Chinese, such as "翼." It has more monosyllabic words than Mandarin, such as "刷," and the word order of compound words can differ from Mandarin, such as "挤拥" and "齐整." It has more loanwords than other dialects, such as "波" (ball), "恤衫" (shirt), and "士多" (store). There are also unique words such as "点解" and "巴闭," and some words come from ancient Chu language, such as "睇" and ancient Zhuang language, such as "谂."
(2) Grammar: Cantonese grammar sometimes places modifiers after the word, such as "你行先." Cantonese has reply forms (叹翻下冷气), continuative forms (食开饭就唔好睇报纸啦), comparative sentences (我大过你), and double-object sentences expressing giving meaning, such as "畀本书我." It also commonly places adjectives after nouns to modify them, such as "水大," "人客," and "鱼生."
(3) Hong Kong Cantonese is more likely to use traditional characters in writing.

Example 1: "今日「衬」大陆银行开门.…脚醒又单拖出发北上.今日在莲塘口岸过关唔多人."
Output format: Cantonese 80%, Mandarin 20%

Example 2: "按导航走走错出口(地图真的不靠谱)"
Output format: Cantonese 20%, Mandarin 80%.

Next, I will provide you with a post to analyze:

```



## 2. Hong Kong-style and Guangdong-style Cantonese Recognition Prompt of LLM

```
You are a language analysis expert. Please determine and output whether the writer is speaking Hong Kong-style Cantonese or Guangdong-style Cantonese. Note:
Hong Kong-style Cantonese (spoken by people in Hong Kong) and Guangdong-style Cantonese (spoken by people in Guangdong) differ in font usage, vocabulary borrowing, sentence structure, topic content, and geographical markers, so please distinguish carefully.

Font usage: Hong Kong-style Cantonese mostly uses traditional characters, while Guangdong-style Cantonese mostly uses simplified characters.

Vocabulary borrowing: Hong Kong-style Cantonese borrows a large number of English words. These borrowed words differ in pronunciation, usage, and meaning compared to Guangdong-style Cantonese.

Code-switching: Hong Kong Cantonese speakers often mix English words or phrases into Cantonese sentences more frequently.

Sentence structure: Hong Kong-style Cantonese more frequently follows English word order or structure.

Output requirements:
Output 1 for Hong Kong-style Cantonese.
Output 0 for Guangdong-style Cantonese.
Example: "請問北上大陆的深圳買计数器和生果，可以過到關回香港嗎, 唔該, thanks."
Analysis: "過到關" is a Cantonese word, "北上," "大陆," "计数器," and "生果" are common terms used by Hong Kong people, involving Hong Kong-related context, and the sentence mixes Cantonese with English.
Output format: 1

Next, please analyze my post.

```

## 3. Prompt for Identifying from a Hong Kong Perspective

```
Determine whether the speaker in this passage is speaking from a Hong Kong perspective, and output 0 or 1.

1 represents a Hong Kong perspective: The place of departure, residence, return, or affiliation is Hong Kong (e.g., going to Shenzhen from Hong Kong, living in Tuen Mun, living in New Territories, living in HK, returning to Hong Kong, going back to HK, returning to Kowloon, etc.). The passage compares the differences between Hong Kong and mainland China from a Hong Kong perspective, uses unique Hong Kong vocabulary (e.g., high tea, working OT, taking a lift, etc., which are mixed Chinese-English expressions uncommon in mainland China), mentions the speaker's identity as a Hong Kong person, or frequently uses traditional Chinese characters for writing.

0 represents a non-Hong Kong perspective: The place of residence is not Hong Kong (e.g., going to Hong Kong, returning to Shenzhen, etc.), and the topic does not reflect a Hong Kong-based perspective.

Note: The passage may discuss topics related to Shenzhen more, but the focus should be on whether it includes a Hong Kong perspective.
Example 1: "Weekend at the border, next week not returning to Shenzhen"
Output format: 0
Example 2: "I have to take the MTR and cross-border buses to Shenzhen for work every day."
Output format: 1

Next, please analyze the example I provide.
```

