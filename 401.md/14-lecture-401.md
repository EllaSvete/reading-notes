# Class 15

## Code Challenge Interview

- getMax()
  - Can i assume anything about the elements?
  - push AND pop
  - as you're pushing things in am i greater than before value?
  - pop out, what was value before?

  - duck duck goose
  - enqueue dequeue a number of times


- sns.set()
- plot_some_lines()
- sns.barplot(x="origin", )
sns.replot(x="year", y = "passengers", data=flights, hue="month")

- year_sums = flights.groupby("year", as_index=False).sum()
sns.relplot(x="year", y="passengers", data=year_sums)

