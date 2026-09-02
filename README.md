# Time_Load_Dual_Back_calibration
An open-source implementation of an alternative adaptive calibration procedure for the Tload task, based on the works . Stimulus duration is individualized based on performance accuracy and response times across a rolling 60-trial window, with separate weighting of numerical and letter-target responses.


This repository provides an open-source PsychoPy implementation of an alternative adaptive calibration procedure for the Tload task. The approach is informed by previous work on Tload task calibration, including the work of Borragan et al. (2016) and the more recent contribution of Hrabovecky (2025).

Building on these approaches, the present implementation explores a response-time-based procedure for individualizing stimulus duration. Rather than relying exclusively on accuracy to determine task difficulty, the procedure incorporates participants' response times on correct, response-required trials. Response times are calculated separately for numerical and letter-target trials and combined using a predefined weighting scheme (35% numerical trials, 65% letter-target trials).

The adaptive procedure operates over successive 60-trial windows. When accuracy exceeds 85%, stimulus duration is adjusted according to the weighted mean response time. When accuracy falls below 70%, stimulus duration is increased by 100 ms. Between these thresholds, stimulus duration remains unchanged.

The goal of this repository is to provide a transparent, reproducible, and accessible implementation of an alternative Tload calibration procedure that can be evaluated and potentially compared with existing calibration approaches.
