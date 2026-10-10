# Seoul Validation Data

This folder contains the Seoul datasets used for the validation and controlled-sample experiments.

| File | Description |
|---|---|
| `val_seoul_data_hts_trip_0.1` | Household travel survey (HTS) trip data sampled at 10% of the ground-truth population. |
| `val_seoul_data_hts_trip_0.2` | HTS trip data sampled at 20% of the ground-truth population. |
| `val_seoul_data_hts_trip_0.4` | HTS trip data sampled at 40% of the ground-truth population. |
| `val_seoul_data_pcm_trip` | Passively collected mobility (PCM) origin–destination–time flow data. |
| `val_seoul_data_true_trip` | Ground-truth trip data in long format. |
| `val_seoul_data_true_tour` | Ground-truth tour data in wide format. |

## Sampled HTS data

The three `val_seoul_data_hts_trip_*` files represent HTS samples retaining 10%, 20%, and 40% of the ground-truth population, respectively. The 100% ground-truth population is the Seoul HTS dataset used in the case studies.

## Ground-truth formats

The ground-truth trip and tour files represent the same underlying population at different levels of organization:

- **Trip format** (`val_seoul_data_true_trip`): long format, with trips represented as records.
- **Tour format** (`val_seoul_data_true_tour`): wide format, with tour information organized across columns.

## PCM data

`val_seoul_data_pcm_trip` contains PCM-derived origin–destination flows indexed by time. It serves as the passively collected mobility data input.
