| **Property**      | **Description**                                               | **Values**                                                                          | **Value Description**                                                                                                                                                          |
| ----------------- | ------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `display`         | Flexbox সক্রিয় করার জন্য ব্যবহৃত হয়।                        | `flex`, `inline-flex`                                                               | `flex`: একটি block-level container।<br>`inline-flex`: একটি inline-level container।                                                                                             |
| `flex-direction`  | Flex items কোন direction-এ থাকবে তা নির্ধারণ করে।             | `row`, `row-reverse`, `column`, `column-reverse`                                    | `row`: Items left-to-right।<br>`row-reverse`: Items right-to-left।<br>`column`: Items top-to-bottom।<br>`column-reverse`: Items bottom-to-top।                                 |
| `flex-wrap`       | Flex items একাধিক লাইনে থাকবে কিনা তা নির্ধারণ করে।           | `nowrap`, `wrap`, `wrap-reverse`                                                    | `nowrap`: Items এক লাইনেই থাকবে।<br>`wrap`: Items একাধিক লাইনে থাকবে।<br>`wrap-reverse`: Items বিপরীত দিকে wrap হবে।                                                           |
| `justify-content` | Main axis বরাবর flex items কিভাবে align হবে তা নির্ধারণ করে।  | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly` | `flex-start`: Items left/top।<br>`flex-end`: Items right/bottom।<br>`center`: Items center।<br>`space-between`: Items মাঝে সমান গ্যাপ।<br>`space-around`: Items চারপাশে গ্যাপ। |
| `align-items`     | Cross axis বরাবর flex items কিভাবে align হবে তা নির্ধারণ করে। | `flex-start`, `flex-end`, `center`, `baseline`, `stretch`                           | `flex-start`: Top aligned।<br>`flex-end`: Bottom aligned।<br>`center`: Centered।<br>`baseline`: Baseline-aligned।<br>`stretch`: Items fit করে।                                 |
| `align-content`   | Multiple lines-এর মধ্যে spacing নির্ধারণ করে।                 | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `stretch`      | `stretch`: Lines পুরো height fit করে।                                                                                                                                          |
| `align-self`      | Individual flex item-এর alignment নির্ধারণ করে।               | `auto`, `flex-start`, `flex-end`, `center`, `baseline`, `stretch`                   | Specific item-এর alignment ওভাররাইড করে।                                                                                                                                       |
| `flex`            | Flex items-এর grow, shrink এবং basis নির্ধারণ করে।            | `<flex-grow> <flex-shrink> <flex-basis>`                                            | উদাহরণ: `1 0 auto`, যা flex-grow এবং flex-shrink নির্ধারণ করে।                                                                                                                 |
| `flex-grow`       | Flex item কতটুকু grow করবে তা নির্ধারণ করে।                   | Non-negative number (e.g., `0`, `1`, `2`)                                           | `1`: Grow করে, `0`: Grow করবে না।                                                                                                                                              |
| `flex-shrink`     | Flex item কতটুকু shrink করবে তা নির্ধারণ করে।                 | Non-negative number (e.g., `0`, `1`, `2`)                                           | `1`: Shrink করে, `0`: Shrink করবে না।                                                                                                                                          |
| `flex-basis`      | Flex item-এর initial size নির্ধারণ করে।                       | `auto`, Length (e.g., `10px`, `50%`)                                                | Initial size set করে।                                                                                                                                                          |
| `order`           | Flex items-এর display order নির্ধারণ করে।                     | Integer values (e.g., `0`, `1`, `-1`)                                               | Default `0`; Positive values: পরে দেখাবে, Negative values: আগে দেখাবে।                                                                                                         |
| `gap`             | Flex items-এর মধ্যে gap নির্ধারণ করে।                         | Length values (e.g., `10px`, `1em`, `%`)                                            | Items এর মধ্যে horizontal এবং vertical gap নির্ধারণ করে।                                                                                                                       |

| **Property**            | **Description**                                                         | **Values**                                                                           | **Value Description**                                                                |
| ----------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `display`               | গ্রিড সক্রিয় করার জন্য ব্যবহৃত হয়।                                    | `grid`, `inline-grid`                                                                | `grid`: Block-level গ্রিড কন্টেইনার।<br>`inline-grid`: Inline-level গ্রিড কন্টেইনার। |
| `grid-template-rows`    | গ্রিডের জন্য প্রতিটি সারির আকার নির্ধারণ করে।                           | Length, Percentage, `auto`, `repeat()`, `minmax()`                                   | প্রতিটি সারির আকার যেমন `100px`, `1fr`, `minmax(100px, auto)` ইত্যাদি।               |
| `grid-template-columns` | গ্রিডের জন্য প্রতিটি কলামের আকার নির্ধারণ করে।                          | Length, Percentage, `auto`, `repeat()`, `minmax()`                                   | প্রতিটি কলামের আকার যেমন `200px`, `1fr`, `minmax(200px, auto)` ইত্যাদি।              |
| `grid-template-areas`   | নামকৃত এলাকা তৈরি করে।                                                  | String values (e.g., `"header header" "sidebar main" "footer footer"`)               | গ্রিড লেআউট নির্ধারণ করে।                                                            |
| `grid-auto-rows`        | অটো-জেনারেটেড সারির আকার নির্ধারণ করে।                                  | Length, Percentage, `auto`, `minmax()`                                               | উদাহরণ: `minmax(100px, auto)`।                                                       |
| `grid-auto-columns`     | অটো-জেনারেটেড কলামের আকার নির্ধারণ করে।                                 | Length, Percentage, `auto`, `minmax()`                                               | উদাহরণ: `200px`।                                                                     |
| `grid-auto-flow`        | অটো-প্লেসমেন্ট এলগরিদমের জন্য নির্ধারণ করে।                             | `row`, `column`, `dense`, `row dense`, `column dense`                                | `row dense`: ঘনভাবে প্লেস করে।                                                       |
| `gap`                   | গ্রিড আইটেমগুলির মধ্যে ফাঁক নির্ধারণ করে।                               | Length values (e.g., `10px`, `1em`, `%`)                                             | সারি এবং কলামের মধ্যে ফাঁক নির্ধারণ করে।                                             |
| `row-gap`               | শুধুমাত্র সারির মধ্যে ফাঁক নির্ধারণ করে।                                | Length values (e.g., `10px`, `1em`)                                                  | সারির মধ্যে নির্দিষ্ট পরিমাণ ফাঁক।                                                   |
| `column-gap`            | শুধুমাত্র কলামের মধ্যে ফাঁক নির্ধারণ করে।                               | Length values (e.g., `10px`, `1em`)                                                  | কলামের মধ্যে নির্দিষ্ট পরিমাণ ফাঁক।                                                  |
| `justify-items`         | গ্রিড আইটেমগুলো main axis বরাবর কিভাবে align হবে তা নির্ধারণ করে।       | `start`, `end`, `center`, `stretch`                                                  | `center`: center-align করে।                                                          |
| `align-items`           | গ্রিড আইটেমগুলো cross axis বরাবর কিভাবে align হবে তা নির্ধারণ করে।      | `start`, `end`, `center`, `stretch`                                                  | `stretch`: Items পুরো height নিয়ে নেবে।                                             |
| `place-items`           | `align-items` এবং `justify-items` এর shorthand প্রপার্টি।               | Combination of `align-items` এবং `justify-items`                                     | উদাহরণ: `center stretch`, যা cross axis-এ center এবং main axis-এ stretch করে।        |
| `justify-content`       | পুরো গ্রিড কন্টেইনার main axis বরাবর কিভাবে align হবে তা নির্ধারণ করে।  | `start`, `end`, `center`, `space-between`, `space-around`, `space-evenly`            | উদাহরণ: `space-between`, যা গ্রিড আইটেমের মাঝে সমান ফাঁক তৈরি করে।                   |
| `align-content`         | পুরো গ্রিড কন্টেইনার cross axis বরাবর কিভাবে align হবে তা নির্ধারণ করে। | `start`, `end`, `center`, `space-between`, `space-around`, `space-evenly`, `stretch` | উদাহরণ: `stretch`, যা পুরো height পূরণ করে।                                          |
| `place-content`         | `align-content` এবং `justify-content` এর shorthand প্রপার্টি।           | Combination of `align-content` এবং `justify-content`                                 | উদাহরণ: `center stretch`।                                                            |
