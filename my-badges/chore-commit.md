<img src="https://my-badges.github.io/my-badges/chore-commit.png" alt="I did a little housekeeping! 🧹" title="I did a little housekeeping! 🧹" width="128">
<strong>I did a little housekeeping! 🧹</strong>
<br><br>

Commits:

- <a href="https://github.com/solusops/StudyBuddy/commit/af8ba5115e15558db5c4736e7914a8c8232a3008">af8ba51</a>: chore: switch to uv + pyproject.toml, remove requirements.txt

Replaces pip/requirements.txt with uv and pyproject.toml. Runtime deps in
[project] dependencies, dev/test deps in [dependency-groups] dev. All run
commands updated to use uv run (uvicorn, pytest). uv.lock committed.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>
Claude-Session: https://claude.ai/code/session_01GooNz7qh4Phx6cjuYxb6DJ


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>