# Commits Against Humanity
## Learning Version Control through Gaming

---

# Background

Cards Against Humanity is a popular card game where a judge presents a prompt card to a group of players. Each player submits a potential answer card, the judge selects the best, or smartest, or funniest one and awards that player a point. Here's an example:
```
> This is the prime of my life. I'm young, hot, and full of ______.
Crippling debt.
```

---

# Variation

Instead of cards, we'll be using the git workflow to play. Here are the modifications we'll be making:

- A prompts will be distributed through a single file in a main repo, which all players will branch
- Players will submit potential answers through a pull request
- The judge will select the best answer and merge it into main
- Play will continue until we get tired
- The player with the most merged branches wins

---

# Workflow 1/2

To submit an answer to a prompt, you will need to:

1. `git checkout main` to switch to the main branch
2. `git pull origin main` to receive the latest master code and prompt
3. `git checkout -b prompt_number_name` to create a new branch for your answer
4. edit the file to add your answer
5. `git add game.md` to stage the changes to your local git repo
6. `git commit -m 'commit message'` to commit those changes to your local repo
7. `git push origin prompt_number_name` to send those changes to github
8. submit a pull request on github.com

---

# Workflow 2/2

This general workflow of checking out main, forking your own branch, committing and pushing changes, and then submitting a pull request is a **very** common workflow that you'll be doing as a software developer. The only difference is that today, you'll be pulling, pushing, and merging very quickly whereas in the real world, it might be days, weeks, or even months between merges.

---

# Let's Play!
