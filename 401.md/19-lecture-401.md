# Class 19

```{python}
def validate(ssn):
    pattern = r"\d{3}-\d{2}-\d{4}"

    match_obj = re.match(pattern, ssn)

    grp = match_obj.group()

    print(grp)

    grp = match_obj.group() if match_obj else None

  return True


goodies = ['111-22-3333`, `222-22-3333`]
baddies = ['666-22-3333', '000-22-333', '900-22-333' ]

for ssn in goodies:
    assert validate(ssn)

```

- is is a good idea to have this team?
- serverless functions for big o questions or something like that
