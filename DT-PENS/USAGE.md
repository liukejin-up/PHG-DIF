# DT-PENS User Guide

You need to also obtain the original PENS dataset at [official website](https://msnews.github.io/pens.html) or [Hugging Face](https://huggingface.co/datasets/THEATLAS/PENS).

## Data Format

### TSV File Structure

The TSV file uses tab characters (`\t`) as delimiters. Each row represents a single user impression (news recommendation session) and contains the following fields:

| Field Name       | Description                                                                 | Example Value |
|------------------|-----------------------------------------------------------------------------|---------------|
| **UserID**       | Unique identifier for the user                                              | `U84844` |
| **ClicknewsID**  | List of news IDs previously clicked by the user, separated by spaces        | `N90215 N109222 N42583 N59544 ... N97484` |
| **dwelltime**    | Dwell times (in seconds) corresponding to each ID in `ClicknewsID`, in the same order, space-separated | `345 633 521 52 ... 19` |
| **exposure_time**| Timestamp when the current news list was exposed to the user                | `7/12/2019 7:02:43 AM` |
| **pos**          | News ID(s) clicked by the user in the current impression (space-separated)  | `N85070 N105901 N19244` |
| **neg**          | News ID(s) displayed but not clicked in the current impression              | `N106268 N97313 N74897 N90052 ...` |
| **start**        | Start timestamp of the current impression session                           | `7/12/2019 7:02:43 AM` |
| **end**          | End timestamp of the current impression session                             | `7/12/2019 7:49:22 AM` |
| **dwelltime_pos**| Dwell time(s) (in seconds) on the news item(s) listed in `pos`, in corresponding order | `687 127 115` |
| **rewrite_titles**| Personalized or rewritten titles for the news items in the current impression, separated by `;;` | `connecticut court to review alex jones case...;;researchers detect high radiation...;;westbrook reunites with harden...` |

