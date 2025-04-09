## Memecoin Analysis Model
![image](https://github.com/user-attachments/assets/6bad7fd9-f34c-4cdb-995d-5b7d0a7a6a94)

![image](https://github.com/user-attachments/assets/d79a71e3-55de-471c-bdcd-eef5597588bb)


### 1. Data Collection and Setup
Dune Analytics Data Retrieval

Connects to Dune Analytics using an API key stored in environment variables

Defines four queries to fetch memecoin performance data across different timeframes:
- 90-day data (query_id: 4948190)
- 30-day data (query_id: 4948159)
- 7-day data (query_id: 4947030)
- 24-hour data (query_id: 4947022)
  
Executes these queries and stores results in separate dataframes.

### 2. Dynamic Market Analysis System
Softmax Weighting Algorithm
- Normalizes importance scores into probability weights that sum to 1
- Ensures numerical stability through max subtraction

Market Condition Detection
- Automatically categorizes the current market state based on relative strength patterns
- Uses standard deviation and ratio analysis to determine market volatility

Dynamic Weight Adjustment
- Adaptively modifies timeframe importance based on current market conditions
- Applies different weighting strategies for each market state

Timeframe Data Combination
- Integrates all timeframe data into a unified analysis framework
- Creates a single ranking that intelligently balances short and long-term performance

### 3. Comparative Analysis System
#### Compares three strategies:
     1. Dynamic weights based on market conditions
     2. Static weights with fixed importance
     3. High volatility scenario emphasizing recent data
- Analyzes how different weighting strategies affect coin rankings
- Identifies coins that appear uniquely in each top 10 list
- Quantifies ranking differences between approaches

### 4. AI-Powered Analysis Engine
Chain-of-Thought Template Generation
- Structures the AI's analytical process for transparency
- Promotes methodical evaluation of coin performance

#### AI Model Creation:
Utilizes the camel-ai framework to create a Gemini 2.0 Flash model instance.

#### Chat Agent Configuration
Creates an AI agent specialized in memecoin analysis

The system message provides:
- The formatted memecoin data
- Current market condition context
- Step-by-step reasoning instructions
- Analysis framework with explicit reasoning requirements

### 5. Insight Generation
The agent analyzes the top memecoins with a structured approach:
- Breaking down timeframe contributions to weighted scores
- Calculating percentage contributions
- Evaluating performance consistency vs. recent momentum
- Comparing coins against each other

### Data Flow Summary
1. Data Collection: Fetch performance metrics across timeframes
2. Market Detection: Analyze patterns to determine market condition
3. Dynamic Weighting: Adjust timeframe importance based on market state
4. Data Integration: Combine weighted data into unified rankings
5. Comparative Analysis: Compare weighting strategies
6. AI Analysis: Feed processed data to AI agent for in-depth insights

This system adapts to changing market conditions and provides transparent, step-by-step analysis of memecoin performance across multiple timeframes, making it valuable for informed investment decisions.
