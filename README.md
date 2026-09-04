# Satsawat Natakarnkitkul (Net)

Data & AI leader in ASEAN. Sixteen years building enterprise AI across banking, telecom, energy, and government in Southeast Asia. I build the AI systems *and* defend the business case for them.

✍ **I write at [satsawat.ai](https://satsawat.ai)**: architecture teardowns, strategy frameworks, and honest accounts of what enterprise AI actually costs and returns.

📬 **Newsletter:** [AI in Practice](https://satsawat.ai/#newsletter), one enterprise AI teardown a month.

## 📚 Books

- **Why Your AI Agent Will Fail**: what the 11% who ship agents to production do differently · [Amazon →](https://www.amazon.com/dp/B0H17XQ9SY)
- **REPLACED**: where your career value lives when AI does the 80% · [Amazon →](https://www.amazon.com/dp/B0H249N4CF)

## 🔧 Selected work

**Studies.** Does it actually work in production, and what does it really cost?

- [tabular-fm-scorecard](https://github.com/netsatsawat/tabular-fm-scorecard): do the new tabular foundation models (big AI models someone else pretrained, then reused for spreadsheet prediction) replace the twenty-year-old standard tool, a gradient-boosted tree you train on your own past rows? Four real business tables, cost measured next to accuracy. The new models tie the tree on accuracy and cost millions of times more per prediction.
- [agent-failure-lab](https://github.com/netsatsawat/agent-failure-lab): an AI agent does a task in many steps, asking a language model (an AI that generates text) once per step. Get each step right 85% of the time and across 10 steps you succeed only 19.7% of the time. Run that math in one command. Then watch it happen on a real 8-step agent, and see how much of the lost success you win back with two fixes: retrying a failed step for free, and paying a second model to check the work. There is a [live calculator](https://netsatsawat.github.io/agent-failure-lab/) too.
- [sovereign-rag](https://github.com/netsatsawat/sovereign-rag): to answer from your own documents, a language model first has to search them, a technique called RAG. Which search wins, keyword (BM25), by-meaning (dense), or a knowledge graph? Everything runs on local models with no cloud, five languages are tested, and every number recomputes from files kept in the repo. One prompt sentence swung a model nearly forty points.
- [agent-report-card](https://github.com/netsatsawat/agent-report-card): a performance review for a bot that answers questions from your own documents. One command, one YAML test file (plain text), one markdown verdict a non-engineer can read. The tool first checks that the grading model is itself reliable, and warns you if you skipped that check. `pip install agent-report-card` · [PyPI](https://pypi.org/project/agent-report-card/), Python's package index
- [tsfm-bakeoff](https://github.com/netsatsawat/tsfm-bakeoff): a fair head-to-head of 13 forecasting methods, five pretrained "foundation" models against eight plain baselines, on ten data series, nine real plus one made-up control to catch cheating. Which one wins at 1, 7, 14 and 30 days ahead? Each model group runs in its own Python environment. Foundation models won 30 of 38 contests.
- [llm-inference-arithmetic](https://github.com/netsatsawat/llm-inference-arithmetic): the back-of-envelope sums to do before you rent GPUs (the chips that run these models) to serve a language model, or before you trust a gap between two benchmark scores (test scores that rate a model). How much memory one conversation eats, how many fit on one GPU, whether the chip is held up waiting for memory or busy doing maths, what a faster piece of code is worth to the whole job, and whether a score gap is real. No GPU needed. A Python library and a command-line tool, no dependencies.
- [did-it-land](https://github.com/netsatsawat/did-it-land): your program charged a customer, then crashed before it could write that down, so on restart it charges again. did-it-land answers two questions before the retry: did the first charge land, and how do you undo it? Four small files cover Stripe (payments), S3 (file storage), GitHub and Postgres (a database).
- [HR-Analytics](https://github.com/netsatsawat/HR-Analytics): predict which staff will quit, on IBM's made-up sample of 1,470 people. Ten models compete, and the best one becomes a ranked call list an HR team can work down. Two more notebooks ask the harder questions. Is the model fair to older staff, and is the test set even big enough to trust the ranking?

**Tutorials.** Fundamentals, built by hand and offline-reproducible.

- [markov-and-hmm](https://github.com/netsatsawat/markov-and-hmm): a Markov model predicts the next state from the current one using one small table of odds. That table can price a loan book, rate an AI agent's odds of finishing, and value a customer. The hidden version, an HMM, works when you cannot see the state directly. Five notebooks that start from zero.
- [fft-seasonality](https://github.com/netsatsawat/fft-seasonality): find the repeating cycles hidden in a stream of measurements, then put them to work. Three notebooks build the Fourier transform by hand (the math that lists those cycles, FFT for short), prove it on sixty-eight years of CO2 (the Keeling curve), and turn hourly demand into a staffing table and an alarm for unusual hours.

📫 hello@satsawat.ai · [LinkedIn](https://www.linkedin.com/in/satsawat/)
