# bihu-tools

## bihu-airdrop-tool.py

1. 币乎官方会给每个合格的参与者, 分配一个奖券号，从1开始的整数。
2. 币乎官方会在空投活动开始前，公布比特币未来的某个区块号，比如1000。 
   - 并使用这个区块的hash，计算一个luck number
   - luck_num = hash1(hash2(...hashn(block.hash)))
3. 对每一个奖券号，计算得分score.
   - score ＝ hash( luck_num + 奖券号) ％ base
4. 依据得分排序，最高的一等奖，以此等等。

Demo:
https://repl.it/@clar1/bihu-airdrop-reward
