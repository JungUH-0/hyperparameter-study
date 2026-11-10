# 결과 문서

단계별 실험 결과를 문서 하나씩 모아 둔다. 노트북은 실행 출력이 비어 있어서 결과는 여기에 기록한다. 요약은 루트 [README](../README.md)의 "결과"에 있다.

| 단계 | 문서 | 상태 |
|---|---|---|
| 2단계 학습률 — 시드 0 훑어보기 (24번) | [step2_learning_rate_seed0.md](step2_learning_rate_seed0.md) | 완료 |
| 2단계 마무리 — 후보 4개 3시드 확인 (16번) | [step2_lr_seeds.md](step2_lr_seeds.md) | 완료 |
| 3단계 Dropout — 시드 0 훑어보기 10번 + 0.5 대 0.75 3시드 확인 8번 | [step3_dropout.md](step3_dropout.md) | 완료 |
| 4단계 에폭 수 (30에폭, 시드 0)와 얼리스탑 채택 | [step4_epochs.md](step4_epochs.md) | 완료 |
| 5단계 증강 — 시드 0 훑어보기 8번 + none 대 rotation 3시드 확인 8번 | [step5_augmentation.md](step5_augmentation.md) | 완료 |
| 6단계 Dropout 재확인 — rotation 기준선에서 0.5 대 0.75, 3시드 6번 | [step6_dropout_recheck.md](step6_dropout_recheck.md) | 완료 |
| 7단계 증강 세 가지를 전부 켠 쪽 대 rotation — 3시드 6번 | [step7_aug_all.md](step7_aug_all.md) | 완료 |

0·1단계와 시드 반복의 결과는 루트 README의 "결과"에 있다.

---

## 새 결과를 추가하는 방법

1. 노트북 마지막 셀의 출력(결과표)과 그래프를 모은다.
2. `단계_내용.md` 형식으로 문서를 만든다 (예: `step2_lr_seeds.md`). 적을 것은 다음과 같다.
   - 어떤 노트북과 조건으로 돌렸는지
   - 결과표
   - 그래프
   - 읽는 법과 관찰
   - 한계
3. 그래프(PNG)는 `figures/`에 둔다. 원자료(CSV)는 `raw/`에 둔다. Colab이 만드는 CSV(`food11_v2_lr.csv`, `food11_v2_seeds.csv`)는 Drive에 쌓이므로 필요하면 내려받아 넣는다. 폴더 이름을 `data/`로 쓰지 않는다. 이 저장소의 `.gitignore`가 `data/`를 무시한다.
4. 위 표와 루트 README의 "진행 상황" 표에 한 줄씩 추가한다.
