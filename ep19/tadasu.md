---
date: 2019-07-25 09:00:00 +0900
layout: blog
title: 3. Neuralinkのまとめ(2019-07-25)
category: blog
author: tadasu
permalink: /blog/3/
---


## 論文
[An integrated brain-machine interface platform with thousands of channels](https://www.biorxiv.org/content/10.1101/703801v1)
- Musk and Neuralink, bioRxiv 2019 ... 今回のNeuralinkの発表とともに公開。メイン論文。科学研究論文というよりは企業が公開するホワイトペーパーという形態である。

[The “sewing machine” for minimally invasive neural recording](https://www.biorxiv.org/content/10.1101/578542v1)
- Hanson et al. bioRxiv 2019 ... 2019年の3月にUCSFから発表されていた論文。ラストオーサーのPhilip Sabesは現在NeuralinkのSenior Scientist。今回の発表の根幹を担う技術についてかなり詳しく述べられている。発表時にNeuralinkとの関係は示されていない。

## YouTube
[Neuralink Launch Event](https://www.youtube.com/watch?v=r-vbh3t7WVI)
- Elon Mask-> Max Hodak->Matt Mcdougall -> Vanessa Tolosa-> DJ Seo -> Philip Sabes -> 質疑応答 (発表内での順番)

## podcast (ep19)
[19. Neuron Musk](https://researchat.fm/episode/19)

## もう少し詳しい資料
[Scrapbox(Musk_bioRxiv_2019)](https://scrapbox.io/researchatfm/Musk_bioRxiv_2019)

## Neuralinkとは
 [Neuralink](https://www.neuralink.com/): 2016年7月に創業、最初の大きな報道は2017年4月
 Elon MuskがOwner
- 1.彼らの最終的な目標、到達点、ゴール
  - 人間とAIを融合させる。
- 2. 現時点での目標
  - 長期間、生体適合性がある侵襲性デバイスの開発
  - 広範囲な脳の領域において、同時に数十万の神経細胞ニューロンの活動を読み書きできる。
- 3. 今回達成したこと
  - "侵襲性"BMIを達成するために必要なNeuralinkの基幹技術の開発(1. threads, 2. robots, 3. electronics, 4. algorithm)
  - Ratにおける実験(読み出しのみ)
  - [質疑応答によると猿でも実験はすすんでいるらしい (コンピューター(カーソル?)をBMIを通して動かすことができるサル)](https://www.msn.com/en-us/video/l/elon-musks-neuralink-reveals-monkey-was-able-to-control-computer-with-its-brain/vp-AAEsApu)
 
## これまで
どうやって脳と機械、コンピューターをつなげるのか。
- BMI(Brain Machine interface)とは
  - 脳内における情報の伝達と処理は神経細胞（ニューロン）の働きによる。
  - ニューロンは電気信号を使って情報伝達する。
  - 脳内に電気信号を読み出したり、電気信号を送り込む、書き込むことによって、脳とコンピュータ、機械とのインタフェースをとなる機器の総称がBMIである。
  - BMIは臨床疾患の広い範囲の人々を助けるポテンシャルがある。
  - コンピューターカーソルの神経補綴(ほてつ)制御やロボットの手足、音声合成装置をデモンストレートしてきた。  
  - BMIは頭蓋骨の開頭を伴う侵襲式と伴わない非侵襲式に大別される。
- 非侵襲式BMIとは(読み出し)
  - 頭皮上に伝わる脳波を゙計測することが可能なEEG(electroencephalogram) ... 数百万のニューロンの情報を頭蓋骨を通して記録することができる。
  - fMRI ... 血流量の増減を指標として脳の広い領域の活動パターンを視覚化する。
  - NIRS ... 近赤外光の透過性を使って血中ヘモグロビン濃度から局所脳活動を 安全に、かつコンパクトな装置で測定可能 (near-infrared optical)
- 非侵襲式BMIの利点と欠点
  - 利点: 非侵襲式では脳を損傷する(および感染症、免疫応答の)リスクが少ないこと、人での研究が比較的容易であること 
  - 欠点: EEGに関しては頭蓋骨などの影響で脳波が歪んでしまうため、侵襲式と比較して空間分解能が劣るなどの問題点がある。そして大量のニューロンのシグナルを平均化した情報しか見れない。

- 侵襲式BMIとは(読み出し)
  - ECoG(electrocorticography) ... 脳表面に電極を貼り付ける皮質脳波の計測()
  - 細胞外記録 ... 脳や脊髄などの組織内の細胞の隙間に電極を差し込んで配置する、もしくは培養細胞に電極を接触させて、神経細胞の近傍に生じる微弱な電気的あるいは電気化学的変化を増幅し記録する方法 
   - 利点:侵襲は正確性と特異性の高い読み取りが可能
   - 欠点: 手術による感染症・脳の損傷といったリスク、電極の経年劣化といった問題点がある。
- BMIによる脳への情報の"書き込み"
  - DBS（Deep Brain  Stimulation：深部脳刺激) ... 侵襲性
  - TMS（Transcranial magnetic stimulation：経頭蓋磁気刺激法) ... 非侵襲性、渦電流によって脳の誘導刺激を行う。

## 発表内容
- 科学的命題
  - BMIによる脳のdecoding研究は大量の数のニューロンからの情報を記録/書き込みできないことによって制限されてきた。

- 解決するべき課題
	 - 大量で広範囲に渡るニューロンの情報を正確に読み書きできる。
	 - 長期間使えて、免疫応答を起こさない。
　- 感染症や脳損傷のリスクがひくい安全な手術方法
  - できるだけ小さく、超低エネルギーで稼働
	 - リアルタイム、かつon-chipで超高速計算できるアルゴリズムとチップの開発 

この問題を1.threads, 2. robots, 3. electornics, 4. algorithmの観点から解決する。


1. Threads (Vanessa Tolosa, Speaker in YouTube)
	極薄微小電極の開発
概要
	活動電位を記録するために最重要なテクノロジーであるが、大きいスケールで記録可能な微小電極の技術はこれまでに無い。

これまで
	多くの長期神経記録のデバイスには硬質な金属や半導体技術によって作られた微小電極アレイが使われてきた。
	硬質な金属は脳にささるが、脳組織の間でミスマッチが免疫応答を駆動させ、これらのデバイスの機能と寿命を制限している。
	アレイの固定形状(例えばユタアレイ)は、血管のせいで、アクセスすることができるニューロンの数を制限する。
要求
	1. 小さくて柔らかい
	2. 高い生体適合性で免疫応答を起こさない
	3. 腐食を起こさないための (airtight packaging)密閉性
	4. 読み出すだけではなく刺激することも可能　(highly functioning BMI)
	5. 製造プロセスがscalableである
	6. そして長い寿命がマテリアルの能力として求められる。
この要求を満たすものはない

アイデア
	代替案は柔らかい、複数の電極ポリマープローブを用いることである。(要は剣山を作るんじゃなくて一本一本埋め込む)。
	この電極ポリマープローブは金属と比べて生体適合性が高い。
	このアプローチの欠点は、薄いポリマープローブは直接脳に挿入できるほど硬くはないため、なんらかの方法で促進する必要がある。そして一本一本植えるので遅い。
		薄いポリマープローブの開発とそれらのプローブを独立に、かつ高速・確実に複数の脳の領域に挿入することができるロボットの開発
	小型化の課題
 	ワイヤーを小さくする。(断面積を小さくする）R =　抵抗率x長さ/断面積
 		抵抗が大きくなる
 			S/Nが悪くなる。
 	Many wires
 		complex　複雑
 			Manufacturing　製造が難しい
 	Tiny electrodes (よくわからん、触れられていない)
 		high stimulation　刺激が大きくなる
			materials and tissue マテリアル&Tissuesの問題
	一つのポリマープローブにたくさんの電極をつける。

