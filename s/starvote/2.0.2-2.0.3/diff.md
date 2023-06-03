# Comparing `tmp/starvote-2.0.2.tar.gz` & `tmp/starvote-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-2.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-2.0.2.tar` & `starvote-2.0.3.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.2/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.2/LICENSE
--rw-r--r--   0        0        0    33924 2023-06-03 00:28:40.930575 starvote-2.0.2/README.md
--rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.2/docs/clarifying_star_voting.md
--rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.2/docs/formatting_fractions_in_columns_of_text.txt
--rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.2/example.py
--rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    89901 2023-06-03 00:25:56.353104 starvote-2.0.2/starvote/__init__.py
--rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.2/starvote/__main__.py
--rw-r--r--   0        0        0     5781 2023-06-02 20:04:16.742802 starvote-2.0.2/starvote/reference.py
--rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.2/test_elections/README.md
--rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.2/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
--rw-r--r--   0        0        0     1358 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.2/test_elections/bad_syntax_change_section_in_list.starvote
--rw-r--r--   0        0        0     1395 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_change_section_in_list.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
--rw-r--r--   0        0        0     1404 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
--rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
--rw-r--r--   0        0        0     1402 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
--rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.2/test_elections/bad_syntax_invalid_method.starvote
--rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_method.txt
--rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.2/test_elections/bad_syntax_invalid_option.starvote
--rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_option.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.2/test_elections/bad_syntax_invalid_pragma.starvote
--rw-r--r--   0        0        0     1376 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_pragma.txt
--rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.2/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
--rw-r--r--   0        0        0     1335 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_start_of_line_mode.txt
--rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_1.starvote
--rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_1.txt
--rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_2.starvote
--rw-r--r--   0        0        0     1360 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_2.txt
--rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.2/test_elections/bad_syntax_invalid_tiebreaker.starvote
--rw-r--r--   0        0        0     1382 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_tiebreaker.txt
--rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.2/test_elections/bad_syntax_malformed_section.starvote
--rw-r--r--   0        0        0     1371 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_malformed_section.txt
--rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.2/test_elections/bad_syntax_no_ballots.starvote
--rw-r--r--   0        0        0     1314 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_ballots.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.2/test_elections/bad_syntax_no_equals.starvote
--rw-r--r--   0        0        0     1346 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_equals.txt
--rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.2/test_elections/bad_syntax_no_method.starvote
--rw-r--r--   0        0        0     1409 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_method.txt
--rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.2/test_elections/bad_syntax_no_section.starvote
--rw-r--r--   0        0        0     1364 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_section.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.2/test_elections/bad_syntax_pragma_in_options.starvote
--rw-r--r--   0        0        0     1375 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_pragma_in_options.txt
--rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.2/test_elections/bad_syntax_pragma_inside_list.starvote
--rw-r--r--   0        0        0     1387 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_pragma_inside_list.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.2/test_elections/bad_syntax_repeated_option.starvote
--rw-r--r--   0        0        0     1380 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_repeated_option.txt
--rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.2/test_elections/bad_syntax_repeated_section.starvote
--rw-r--r--   0        0        0     1383 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_repeated_section.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
--rw-r--r--   0        0        0     1403 2023-06-03 00:24:26.576301 starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
--rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
--rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
--rw-r--r--   0        0        0     3193 2023-06-03 00:24:26.584301 starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.pdf
--rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.588301 starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
--rw-r--r--   0        0        0     2879 2023-06-03 00:24:26.592301 starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
--rw-r--r--   0        0        0     1596 2023-06-03 00:24:26.612301 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
--rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
--rw-r--r--   0        0        0    12586 2023-06-03 00:24:26.932304 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
--rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
--rw-r--r--   0        0        0    12586 2023-06-03 00:24:27.260307 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.pdf
--rw-r--r--   0        0        0      814 2023-06-03 00:24:27.264307 starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
--rw-r--r--   0        0        0      799 2023-06-03 00:24:27.264307 starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
--rw-r--r--   0        0        0     1434 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
--rw-r--r--   0        0        0      747 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.2/test_elections/test_election_all_fives_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/test_election_all_fives_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.2/test_elections/test_election_all_fives_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/test_election_all_fives_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.2/test_elections/test_election_all_fives_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_fives_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.2/test_elections/test_election_all_fives_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_fives_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.2/test_elections/test_election_all_threes_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_bloc_star.txt
--rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.2/test_elections/test_election_all_threes_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_rrv.txt
--rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.2/test_elections/test_election_all_threes_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.2/test_elections/test_election_all_threes_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.2/test_elections/test_election_all_zeroes_bloc_star.starvote
--rw-r--r--   0        0        0     1077 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.2/test_elections/test_election_all_zeroes_rrv.starvote
--rw-r--r--   0        0        0      481 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.2/test_elections/test_election_all_zeroes_star-pr.starvote
--rw-r--r--   0        0        0      473 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.2/test_elections/test_election_all_zeroes_star.starvote
--rw-r--r--   0        0        0     1027 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_star.txt
--rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.starvote
--rw-r--r--   0        0        0     3383 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.txt
--rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
--rw-r--r--   0        0        0     1606 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
--rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.2/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      831 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
--rw-r--r--   0        0        0      965 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
--rw-r--r--   0        0        0      744 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
--rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.starvote
--rw-r--r--   0        0        0      542 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.txt
--rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.starvote
--rw-r--r--   0        0        0     1087 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.txt
--rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.2/test_elections/test_election_extra_candidates_in_permutation.starvote
--rw-r--r--   0        0        0      142 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_extra_candidates_in_permutation.txt
--rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.2/test_elections/test_election_incomplete_permutation.starvote
--rw-r--r--   0        0        0      138 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_incomplete_permutation.txt
--rw-r--r--   0        0        0      132 2023-06-02 01:44:01.610291 starvote-2.0.2/test_elections/test_election_no_output.starvote
--rw-r--r--   0        0        0       17 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_no_output.txt
--rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.2/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
--rw-r--r--   0        0        0     1329 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
--rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.2/test_elections/test_election_only_one_candidate_star.starvote
--rw-r--r--   0        0        0      505 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_one_candidate_star.txt
--rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.2/test_elections/test_election_only_two_candidates_bloc_star.starvote
--rw-r--r--   0        0        0      487 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_two_candidates_bloc_star.txt
--rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.2/test_elections/test_election_only_two_candidates_rrv.starvote
--rw-r--r--   0        0        0      523 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_two_candidates_rrv.txt
--rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.2/test_elections/test_election_only_two_candidates_star-pr.starvote
--rw-r--r--   0        0        0      545 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_two_candidates_star-pr.txt
--rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.2/test_elections/test_election_proportional_star_unbreakable_tie.starvote
--rw-r--r--   0        0        0      480 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_proportional_star_unbreakable_tie.txt
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.html
--rw-r--r--   0        0        0      450 2023-05-31 14:05:31.788268 starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.starvote
--rw-r--r--   0        0        0     1150 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
--rw-r--r--   0        0        0     1023 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
--rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0     1788 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
--rw-r--r--   0        0        0     2029 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.2/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      938 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.2/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
--rw-r--r--   0        0        0     1081 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
--rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.2/test_elections/test_election_use_just_raise_tiebreaker.starvote
--rw-r--r--   0        0        0     1103 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_use_just_raise_tiebreaker.txt
--rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.2/test_elections/test_election_use_no_description_tiebreaker.starvote
--rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_use_no_description_tiebreaker.txt
--rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.2/test_elections/test_election_use_only_heading_tiebreaker.starvote
--rw-r--r--   0        0        0      152 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_use_only_heading_tiebreaker.txt
--rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.2/tests/harness.py
--rw-r--r--   0        0        0    35844 2023-06-03 00:26:24.333354 starvote-2.0.2/tests/run_tests.py
--rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.2/tools/is_ok
--rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.2/tools/remake_test_elections_output
--rw-r--r--   0        0        0    34494 1970-01-01 00:00:00.000000 starvote-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.3/LICENSE
+-rw-r--r--   0        0        0    34907 2023-06-03 01:10:41.133110 starvote-2.0.3/README.md
+-rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.3/docs/clarifying_star_voting.md
+-rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.3/docs/formatting_fractions_in_columns_of_text.txt
+-rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.3/example.py
+-rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    89957 2023-06-03 00:56:46.533647 starvote-2.0.3/starvote/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.3/starvote/__main__.py
+-rw-r--r--   0        0        0     5872 2023-06-03 01:02:33.216747 starvote-2.0.3/starvote/reference.py
+-rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.3/test_elections/README.md
+-rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.3/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
+-rw-r--r--   0        0        0     1358 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.3/test_elections/bad_syntax_change_section_in_list.starvote
+-rw-r--r--   0        0        0     1395 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_change_section_in_list.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
+-rw-r--r--   0        0        0     1404 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
+-rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
+-rw-r--r--   0        0        0     1402 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
+-rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.3/test_elections/bad_syntax_invalid_method.starvote
+-rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_method.txt
+-rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.3/test_elections/bad_syntax_invalid_option.starvote
+-rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_option.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.3/test_elections/bad_syntax_invalid_pragma.starvote
+-rw-r--r--   0        0        0     1376 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_pragma.txt
+-rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.3/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
+-rw-r--r--   0        0        0     1335 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_start_of_line_mode.txt
+-rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_1.starvote
+-rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_1.txt
+-rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_2.starvote
+-rw-r--r--   0        0        0     1360 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_2.txt
+-rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.3/test_elections/bad_syntax_invalid_tiebreaker.starvote
+-rw-r--r--   0        0        0     1382 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_tiebreaker.txt
+-rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.3/test_elections/bad_syntax_malformed_section.starvote
+-rw-r--r--   0        0        0     1371 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_malformed_section.txt
+-rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.3/test_elections/bad_syntax_no_ballots.starvote
+-rw-r--r--   0        0        0     1314 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_ballots.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.3/test_elections/bad_syntax_no_equals.starvote
+-rw-r--r--   0        0        0     1346 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_equals.txt
+-rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.3/test_elections/bad_syntax_no_method.starvote
+-rw-r--r--   0        0        0     1409 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_method.txt
+-rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.3/test_elections/bad_syntax_no_section.starvote
+-rw-r--r--   0        0        0     1364 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_section.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.3/test_elections/bad_syntax_pragma_in_options.starvote
+-rw-r--r--   0        0        0     1375 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_pragma_in_options.txt
+-rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.3/test_elections/bad_syntax_pragma_inside_list.starvote
+-rw-r--r--   0        0        0     1387 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_pragma_inside_list.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.3/test_elections/bad_syntax_repeated_option.starvote
+-rw-r--r--   0        0        0     1380 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_repeated_option.txt
+-rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.3/test_elections/bad_syntax_repeated_section.starvote
+-rw-r--r--   0        0        0     1383 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_repeated_section.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
+-rw-r--r--   0        0        0     1403 2023-06-03 00:24:26.576301 starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
+-rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
+-rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
+-rw-r--r--   0        0        0     3193 2023-06-03 00:24:26.584301 starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.pdf
+-rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.588301 starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
+-rw-r--r--   0        0        0     2879 2023-06-03 00:24:26.592301 starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
+-rw-r--r--   0        0        0     1596 2023-06-03 00:24:26.612301 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
+-rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
+-rw-r--r--   0        0        0    12586 2023-06-03 00:24:26.932304 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
+-rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
+-rw-r--r--   0        0        0    12586 2023-06-03 00:24:27.260307 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.pdf
+-rw-r--r--   0        0        0      814 2023-06-03 00:24:27.264307 starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
+-rw-r--r--   0        0        0      799 2023-06-03 00:24:27.264307 starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
+-rw-r--r--   0        0        0     1434 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
+-rw-r--r--   0        0        0      747 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.3/test_elections/test_election_all_fives_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/test_election_all_fives_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.3/test_elections/test_election_all_fives_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/test_election_all_fives_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.3/test_elections/test_election_all_fives_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_fives_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.3/test_elections/test_election_all_fives_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_fives_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.3/test_elections/test_election_all_threes_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_bloc_star.txt
+-rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.3/test_elections/test_election_all_threes_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_rrv.txt
+-rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.3/test_elections/test_election_all_threes_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.3/test_elections/test_election_all_threes_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.3/test_elections/test_election_all_zeroes_bloc_star.starvote
+-rw-r--r--   0        0        0     1077 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.3/test_elections/test_election_all_zeroes_rrv.starvote
+-rw-r--r--   0        0        0      481 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.3/test_elections/test_election_all_zeroes_star-pr.starvote
+-rw-r--r--   0        0        0      473 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.3/test_elections/test_election_all_zeroes_star.starvote
+-rw-r--r--   0        0        0     1027 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_star.txt
+-rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.starvote
+-rw-r--r--   0        0        0     3383 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.txt
+-rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
+-rw-r--r--   0        0        0     1606 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
+-rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.3/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      831 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
+-rw-r--r--   0        0        0      965 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
+-rw-r--r--   0        0        0      744 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
+-rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.starvote
+-rw-r--r--   0        0        0      542 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.txt
+-rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.starvote
+-rw-r--r--   0        0        0     1087 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.txt
+-rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.3/test_elections/test_election_extra_candidates_in_permutation.starvote
+-rw-r--r--   0        0        0      142 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_extra_candidates_in_permutation.txt
+-rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.3/test_elections/test_election_incomplete_permutation.starvote
+-rw-r--r--   0        0        0      138 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_incomplete_permutation.txt
+-rw-r--r--   0        0        0      132 2023-06-03 00:43:08.954337 starvote-2.0.3/test_elections/test_election_no_output.starvote
+-rw-r--r--   0        0        0       17 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_no_output.txt
+-rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.3/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
+-rw-r--r--   0        0        0     1329 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
+-rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.3/test_elections/test_election_only_one_candidate_star.starvote
+-rw-r--r--   0        0        0      505 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_one_candidate_star.txt
+-rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.3/test_elections/test_election_only_two_candidates_bloc_star.starvote
+-rw-r--r--   0        0        0      487 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_two_candidates_bloc_star.txt
+-rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.3/test_elections/test_election_only_two_candidates_rrv.starvote
+-rw-r--r--   0        0        0      523 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_two_candidates_rrv.txt
+-rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.3/test_elections/test_election_only_two_candidates_star-pr.starvote
+-rw-r--r--   0        0        0      545 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_two_candidates_star-pr.txt
+-rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.3/test_elections/test_election_proportional_star_unbreakable_tie.starvote
+-rw-r--r--   0        0        0      480 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_proportional_star_unbreakable_tie.txt
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.html
+-rw-r--r--   0        0        0      450 2023-06-03 00:37:52.439507 starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.starvote
+-rw-r--r--   0        0        0     1150 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
+-rw-r--r--   0        0        0     1023 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
+-rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0     1788 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
+-rw-r--r--   0        0        0     2029 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.3/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      938 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.3/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
+-rw-r--r--   0        0        0     1081 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
+-rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.3/test_elections/test_election_use_just_raise_tiebreaker.starvote
+-rw-r--r--   0        0        0     1103 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_use_just_raise_tiebreaker.txt
+-rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.3/test_elections/test_election_use_no_description_tiebreaker.starvote
+-rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_use_no_description_tiebreaker.txt
+-rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.3/test_elections/test_election_use_only_heading_tiebreaker.starvote
+-rw-r--r--   0        0        0      152 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_use_only_heading_tiebreaker.txt
+-rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.3/tests/harness.py
+-rw-r--r--   0        0        0    36446 2023-06-03 01:08:39.424022 starvote-2.0.3/tests/run_tests.py
+-rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.3/tools/is_ok
+-rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.3/tools/remake_test_elections_output
+-rw-r--r--   0        0        0    35477 1970-01-01 00:00:00.000000 starvote-2.0.3/PKG-INFO
```

### Comparing `starvote-2.0.2/LICENSE` & `starvote-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/README.md` & `starvote-2.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -181,24 +181,29 @@
 ```
 
 `election` tabulates an election based on your
 parameter and returns a `list` containing the
 winners. (Even for single-winner STAR Voting--in
 that case, the list will only contain one element.)
 
-`method` specifies which election system you want to use.
-The allowed values are
-`starvote.STAR_Voting`,
-`starvote.Bloc_STAR_Voting`,
-`starvote.Allocated_Score_Voting`,
-and
-`starvote.Reweighted_Range_Voting`.  (Since those are a lot to
+`method` specifies which election system you want to use,
+via predefined `Method` objects. The allowed values are:
+
+* `starvote.STAR_Voting`,
+* `starvote.Bloc_STAR_Voting`,
+* `starvote.Allocated_Score_Voting`, and
+* `starvote.Reweighted_Range_Voting`.
+
+Since those are a lot to
 type, `starvote` also provides nicknames, respectively:
-`starvote.star`, `starvote.bloc`, `starvote.allocated`,
-and `starvote.rrv`.)
+
+* `starvote.star`,
+* `starvote.bloc`,
+* `starvote.allocated`, and
+* `starvote.rrv`.
 
 `ballots` should be an iterable containing individual ballots.
 Ballots are `dict` objects, mapping the candidate to that ballot's
 score for that candidate.  The candidate can be any Python value;
 the score must be an `int`.
 
 `maximum_score` specifies the maximum score allowed for any vote
@@ -250,24 +255,35 @@
 `starvote` ships a copy of the reference implementation
 of Allocated Score Voting.  Since this requires both NumPy
 and Pandas, it's not imported by default.  (I didn't want
 `starvote` to have any external dependencies.  The unit
 test suite runs correctly whether or not these external
 dependencies are installed.)
 
-You can import it with `import starvote.reference`,
-and you can integrate it into the `starvote` module by
-calling `starvote.reference.monkey_patch()`.  Its
-implementation function can be found at
-`starvote.reference.allocated_score_voting_reference`,
-and it's added to `methods` under the name
-`'Allocated Score Voting (reference)'`.
+You can import it with `import starvote.reference`;
+the directly-callable function is
+`starvote.reference.allocated_score_voting_reference`.
+You can also use the `Method` object
+
+If you want to integrate it into the `starvote` module,
+call`starvote.reference.monkey_patch()`.  This does
+three things:
+
+* Adds the function to the `starvote` module directly,
+  as `starvote.allocated_score_voting_reference`.
+* Adds it to `starvote.__all__` so that symbol
+  gets brought in by `from starvote import *`.
+*
+* Adds the appropriate `Method` object
+  to `starvote.methods`, using the name
+  `'Allocated Score Voting (reference)'`
+  and the nickname `allocated_r`.
 
 *Note:* the reference implementation doesn't support
-tiebreakers.  `allocated_score_voting_reference` does
+tiebreakers.  `allocated_score_voting_reference` *does*
 accept a `tiebreaker` argument, but currently it *must*
 be `None`.
 
 ### Ties
 
 The good news is, STAR Voting elections rarely result in a tie in the
 real world.  But ties can still happen.  The good news is, STAR Voting
@@ -723,15 +739,15 @@
 
 You can experiment with these with the command-line version of the
 module, too.  You can specify the electoral system with `-e`,
 the number of seats with `-s`,
 and the maximum score with `-m`:
 
 ```
-% python3 -m starvote -e Reweighted_Range -s 3 -m 10 sample_polls/sample_poll_reweighted_range_3_seats.csv
+% python3 -m starvote test_elections/test_election_reweighted_range_sample_election.starvote
 ```
 
 ### Warning
 
 I haven't found a single test corpus for Bloc STAR Voting.
 I'm following the rules as best I can, and the results I'm getting
 make sense.  But so far I can't confirm my implementation is
@@ -773,14 +789,30 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.3** - *2023/05/27*
+
+* Normalized nomenclature for `Method` objects.  Now,
+  every method has an official correctly-spelled
+  correctly-capitalized name, and exactly one "nickname".
+  The nickname is always lowercase, and would return
+  True for `isidentifier`.  These are used in the
+  `starvote.method` map; a variant of these names is
+  also bound as module attributes (changed so they're
+  valid identifiers).
+* Improved `starvote.reference.monkey_patch`.  It's now
+  data-driven and thus more reliable.
+* Added `starvote.reference.__all__`, in case you want
+  to `from starvote.reference import *`.
+* Doc fixes.
+
 **2.0.2** - *2023/05/27*
 
 * Renamed the `tiebreaker` parameter `candidates` to `tie`.
 * Evicted some testing-only tiebreakers from the `starvote`
   module.  They're now in their own script, which only gets
   loaded when working with the test suite.
```

### Comparing `starvote-2.0.2/docs/clarifying_star_voting.md` & `starvote-2.0.3/docs/clarifying_star_voting.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/docs/formatting_fractions_in_columns_of_text.txt` & `starvote-2.0.3/docs/formatting_fractions_in_columns_of_text.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/pyproject.toml` & `starvote-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/starvote/__init__.py` & `starvote-2.0.3/starvote/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python3
 
 ##
 ## TODO
 ##
-## * write a unit test that confirms "example.py"
-##   runs, and the output in README.md is up to date
-##   (I keep breaking it / its output keeps getting outdated.)
+## * write a unit test that checks the code examples
+##   in README.md are up to date
+##     * confirms "example.py" and the output in README.md matches
+##     * confirms the "multi-winner elections" cmdline works
+##   (I keep breaking these.)
 ##
 
 __doc__ = "An election tabulator for the STAR electoral system, and others"
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 __all__ = [
     'Allocated_Score_Voting', # Method
-    'Allocated', # Method (nickname)
+    'allocated', # Method (nickname)
     'allocated_score_voting', # function
     'Bloc_STAR_Voting', # Method
-    'Bloc', # Method (nickname)
+    'bloc', # Method (nickname)
     'bloc_star_voting', # function
     'Method', # class for method metadata
     'methods', # maps string to Methods
     'load_starvote_file', # function
     'main', # function
     'Options', # class
     'predefined_permutation_tiebreaker', # tiebreaker class
     'parse_starvote', # function
     'on_demand_random_tiebreaker', # tiebreaker function
     'Reweighted_Range_Voting', # Method
-    'RRV', # Method (nickname)
+    'rrv', # Method (nickname)
     'reweighted_range_voting', # function
     'STAR_Voting', # Method
-    'STAR', # Method (name)
+    'star', # Method (name)
     'star_voting', # function
     'Tiebreaker', # class
     'tiebreakers', # maps string to tiebreakers
     'UnbreakableTieError', # exception class
     'UsageException', # exception class
     ]
 
@@ -1362,16 +1364,16 @@
         tie = None
     except UnbreakableTieError as e:
         winners = None
         tie = e
     return options.election_result(winners, tie)
 
 
-STAR_Voting = STAR = Method("STAR Voting", star_voting, False)
-for _ in ('STAR Voting', 'STAR', 'star'):
+STAR_Voting = star = Method("STAR Voting", star_voting, False)
+for _ in ('STAR Voting', 'star'):
     methods[_] = STAR_Voting
 
 
 
 def bloc_star_voting(ballots, *,
     maximum_score=_DEFAULT_MAXIMUM_SCORE,
     print=_DEFAULT_PRINT,
@@ -1438,16 +1440,16 @@
 
         tie = None
     except UnbreakableTieError as e:
         winners = None
         tie = e
     return options.election_result(winners, tie)
 
-Bloc = Bloc_STAR_Voting = Method("Bloc STAR", bloc_star_voting, True)
-for _ in ('Bloc STAR Voting', 'Bloc', 'bloc'):
+Bloc_STAR_Voting = bloc = Method("Bloc STAR", bloc_star_voting, True)
+for _ in ('Bloc STAR Voting', 'bloc'):
     methods[_] = Bloc_STAR_Voting
 
 
 
 def allocated_score_voting(ballots, *,
     maximum_score=_DEFAULT_MAXIMUM_SCORE,
     print=_DEFAULT_PRINT,
@@ -1683,16 +1685,16 @@
         _attempt_to_sort(winners)
         tie = None
     except UnbreakableTieError as e:
         winners = None
         tie = e
     return options.election_result(winners, tie)
 
-Allocated_Score_Voting = Allocated = Method("Allocated Score Voting", allocated_score_voting, True)
-for _ in ('Allocated Score Voting', 'Allocated', 'allocated'):
+Allocated_Score_Voting = allocated = Method("Allocated Score Voting", allocated_score_voting, True)
+for _ in ('Allocated Score Voting', 'allocated'):
     methods[_] = Allocated_Score_Voting
 
 
 
 def reweighted_range_voting(ballots, *,
     maximum_score=_DEFAULT_MAXIMUM_SCORE,
     print=_DEFAULT_PRINT,
@@ -1824,16 +1826,16 @@
         _attempt_to_sort(winners)
         tie = None
     except UnbreakableTieError as e:
         winners = None
         tie = e
     return options.election_result(winners, tie)
 
-Reweighted_Range_Voting = RRV = Method("Reweighted Range Voting", reweighted_range_voting, True)
-for _ in ('Reweighted Range Voting', 'RRV', 'rrv'):
+Reweighted_Range_Voting = rrv = Method("Reweighted Range Voting", reweighted_range_voting, True)
+for _ in ('Reweighted Range Voting', 'rrv'):
     methods[_] = Reweighted_Range_Voting
 
 
 def election(method, ballots, *,
     maximum_score=_DEFAULT_MAXIMUM_SCORE,
     print=_DEFAULT_PRINT,
     seats=_DEFAULT_SEATS,
@@ -2469,15 +2471,15 @@
         raise UsageException("no csv or starvote file specified.")
     if not path.is_file():
         raise UsageException(f"invalid file specified: {path}")
 
     def load_election_from_csv_file(path):
         return {
             'ballots': load_csv_file(path),
-            'method': STAR,
+            'method': STAR_Voting,
             'verbosity': 1,
             'tiebreaker': None,
             }
 
     extension = path.suffix
     loader = {
         '.csv': load_election_from_csv_file,
@@ -2529,15 +2531,15 @@
         # s = repr(e)
         name = e.__class__.__name__
         s = f"{name}({repr(str(e))})"
         text_print(s)
 
     if (winners or tie) and (not kwargs.get('verbosity', 0)):
         # no output!  print the results ourselves.
-        fake_options = Options(STAR, print=text_print, verbosity=1, seats=1, tiebreaker=None, maximum_score=5)
+        fake_options = Options(STAR_Voting, print=text_print, verbosity=1, seats=1, tiebreaker=None, maximum_score=5)
         fake_options.election_result(winners, tie, raise_tie=False)
 
     s = text_getvalue()
     if s: # pragma: no cover
         print(s, end='')
 
     return 0
```

### Comparing `starvote-2.0.2/starvote/reference.py` & `starvote-2.0.3/starvote/reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,24 +145,33 @@
         print(f"[Winner{plural}]")
         for winner in winner_names:
             print(f"  {winners}")
 
     return winners
 
 
-Allocated_Score_Voting_reference = starvote.Method("Allocated Score Voting (reference)", allocated_score_voting_reference, True)
+Allocated_Score_Voting_reference = allocated_r = starvote.Method("Allocated Score Voting (reference)", allocated_score_voting_reference, True)
+methods = {
+    'Allocated Score Voting (reference)': Allocated_Score_Voting_reference,
+    'allocated_r': Allocated_Score_Voting_reference,
+    }
+
+__all__ = [
+    "Allocated_Score_Voting_reference", # Method
+    "allocated_r", # Method (nickname)
+    "allocated_score_voting_reference", # function
+    ]
 
 def monkey_patch():
     """
     Adds the reference implementation of Proportional STAR from the STAR voting website
     to the available electoral systems provided by starvote, under the name
     'Reference Proportional STAR'.
     """
-    for name in (
-        'Allocated Score Voting (reference)',
-        'Allocated-R',
-        'allocated-r',
-        ):
-        starvote.methods[name] = Allocated_Score_Voting_reference
-    starvote.Allocated_Score_Voting_reference = Allocated_Score_Voting_reference
-    starvote.allocated_score_voting_reference = allocated_score_voting_reference
-    starvote.__all__.append('Allocated_Score_Voting_reference')
+    starvote.methods.update(methods)
+
+    g = globals()
+
+    for name in __all__:
+        symbol = g[name]
+        setattr(starvote, name, symbol)
+        starvote.__all__.append(name)
```

### Comparing `starvote-2.0.2/test_elections/README.md` & `starvote-2.0.3/test_elections/README.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_ballot_pragma_as_last_line.txt` & `starvote-2.0.3/test_elections/bad_syntax_ballot_pragma_as_last_line.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_change_section_in_list.txt` & `starvote-2.0.3/test_elections/bad_syntax_change_section_in_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_1.txt` & `starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_2.txt` & `starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_method.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_option.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_pragma.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_pragma.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_start_of_line_mode.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_start_of_line_mode.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_1.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_2.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_invalid_tiebreaker.txt` & `starvote-2.0.3/test_elections/bad_syntax_invalid_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_malformed_section.txt` & `starvote-2.0.3/test_elections/bad_syntax_malformed_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_no_ballots.txt` & `starvote-2.0.3/test_elections/bad_syntax_no_ballots.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_no_equals.txt` & `starvote-2.0.3/test_elections/bad_syntax_no_equals.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_no_method.txt` & `starvote-2.0.3/test_elections/bad_syntax_no_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_no_section.txt` & `starvote-2.0.3/test_elections/bad_syntax_no_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_pragma_in_options.txt` & `starvote-2.0.3/test_elections/bad_syntax_pragma_in_options.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_pragma_inside_list.txt` & `starvote-2.0.3/test_elections/bad_syntax_pragma_inside_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_repeated_option.txt` & `starvote-2.0.3/test_elections/bad_syntax_repeated_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/bad_syntax_repeated_section.txt` & `starvote-2.0.3/test_elections/bad_syntax_repeated_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt` & `starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv` & `starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt` & `starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.csv` & `starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.txt` & `starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.txt` & `starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt` & `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt` & `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt` & `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.csv` & `starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.txt` & `starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.txt` & `starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt` & `starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf` & `starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt` & `starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_all_fives_bloc_star.txt` & `starvote-2.0.3/test_elections/test_election_all_fives_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_all_fives_star.txt` & `starvote-2.0.3/test_elections/test_election_all_fives_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_all_threes_bloc_star.txt` & `starvote-2.0.3/test_elections/test_election_all_threes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_all_threes_star.txt` & `starvote-2.0.3/test_elections/test_election_all_threes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_all_zeroes_bloc_star.txt` & `starvote-2.0.3/test_elections/test_election_all_zeroes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_all_zeroes_star.txt` & `starvote-2.0.3/test_elections/test_election_all_zeroes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.starvote` & `starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.txt` & `starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote` & `starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt` & `starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_breakable_tie_for_second_in_score_round.txt` & `starvote-2.0.3/test_elections/test_election_breakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt` & `starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt` & `starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.starvote` & `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.txt` & `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.starvote` & `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.txt` & `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_no_permuted_candidates_tiebreaker.txt` & `starvote-2.0.3/test_elections/test_election_no_permuted_candidates_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_only_two_candidates_rrv.txt` & `starvote-2.0.3/test_elections/test_election_only_two_candidates_rrv.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_only_two_candidates_star-pr.txt` & `starvote-2.0.3/test_elections/test_election_only_two_candidates_star-pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.html` & `starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.html`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.txt` & `starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt` & `starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt` & `starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt` & `starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt` & `starvote-2.0.3/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt` & `starvote-2.0.3/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_use_just_raise_tiebreaker.txt` & `starvote-2.0.3/test_elections/test_election_use_just_raise_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/test_elections/test_election_use_no_description_tiebreaker.txt` & `starvote-2.0.3/test_elections/test_election_use_no_description_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/tests/harness.py` & `starvote-2.0.3/tests/harness.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/tests/run_tests.py` & `starvote-2.0.3/tests/run_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,19 +143,32 @@
         C = 4
 """
 
 
 class StarvoteTests(unittest.TestCase):
 
     def test_import_star(self):
-        module = "from starvote import *"
+        # test that import * works
+        # (it will fail if there's a bug with the definition of __all__)
 
+        # test should still work even if we can't load numpy / pandas
+        try:
+            import starvote.reference
+            module = "import starvote.reference\nstarvote.reference.monkey_patch()\ndel starvote\nfrom starvote import *"
+            reference_imported_ok = True
+        except ImportError: # pragma: no cover
+            module = "from starvote import *"
+            reference_imported_ok = False
+
+        import starvote
         g = {}
         exec(module, g, g)
         self.assertEqual(g['STAR_Voting'], starvote.STAR_Voting)
+        if reference_imported_ok:
+            self.assertEqual(g['allocated_r'], starvote.reference.allocated_r)
 
     def test_random_tiebreaker(self):
         election = tied_election.format(options="tiebreaker = on_demand_random_tiebreaker")
         kwargs = starvote.parse_starvote(election)
 
         text_clear, text_print, text_getvalue = starvote._printer()
         result = starvote.election(**kwargs, print=text_print)
@@ -370,15 +383,15 @@
         self.assertEqual(results, ['Amy', 'Chuck', 'Darcy'])
 
         try :
             from starvote import reference
         except ImportError: # pragma: no cover
             return
 
-        kwargs['method'] = reference.Allocated_Score_Voting_reference
+        kwargs['method'] = reference.allocated_r
         kwargs['tiebreaker'] = None
         reference_results = starvote.election(**kwargs)
         self.assertEqual(reference_results, results)
 
     def test_fraction_formatting(self):
         for i, t in (
             (1, ('1', '', '', '') ),
```

### Comparing `starvote-2.0.2/tools/is_ok` & `starvote-2.0.3/tools/is_ok`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/tools/remake_test_elections_output` & `starvote-2.0.3/tools/remake_test_elections_output`

 * *Files identical despite different names*

### Comparing `starvote-2.0.2/PKG-INFO` & `starvote-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 2.0.2
+Version: 2.0.3
 Summary: An election tabulator for the STAR electoral system, and others
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -196,24 +196,29 @@
 ```
 
 `election` tabulates an election based on your
 parameter and returns a `list` containing the
 winners. (Even for single-winner STAR Voting--in
 that case, the list will only contain one element.)
 
-`method` specifies which election system you want to use.
-The allowed values are
-`starvote.STAR_Voting`,
-`starvote.Bloc_STAR_Voting`,
-`starvote.Allocated_Score_Voting`,
-and
-`starvote.Reweighted_Range_Voting`.  (Since those are a lot to
+`method` specifies which election system you want to use,
+via predefined `Method` objects. The allowed values are:
+
+* `starvote.STAR_Voting`,
+* `starvote.Bloc_STAR_Voting`,
+* `starvote.Allocated_Score_Voting`, and
+* `starvote.Reweighted_Range_Voting`.
+
+Since those are a lot to
 type, `starvote` also provides nicknames, respectively:
-`starvote.star`, `starvote.bloc`, `starvote.allocated`,
-and `starvote.rrv`.)
+
+* `starvote.star`,
+* `starvote.bloc`,
+* `starvote.allocated`, and
+* `starvote.rrv`.
 
 `ballots` should be an iterable containing individual ballots.
 Ballots are `dict` objects, mapping the candidate to that ballot's
 score for that candidate.  The candidate can be any Python value;
 the score must be an `int`.
 
 `maximum_score` specifies the maximum score allowed for any vote
@@ -265,24 +270,35 @@
 `starvote` ships a copy of the reference implementation
 of Allocated Score Voting.  Since this requires both NumPy
 and Pandas, it's not imported by default.  (I didn't want
 `starvote` to have any external dependencies.  The unit
 test suite runs correctly whether or not these external
 dependencies are installed.)
 
-You can import it with `import starvote.reference`,
-and you can integrate it into the `starvote` module by
-calling `starvote.reference.monkey_patch()`.  Its
-implementation function can be found at
-`starvote.reference.allocated_score_voting_reference`,
-and it's added to `methods` under the name
-`'Allocated Score Voting (reference)'`.
+You can import it with `import starvote.reference`;
+the directly-callable function is
+`starvote.reference.allocated_score_voting_reference`.
+You can also use the `Method` object
+
+If you want to integrate it into the `starvote` module,
+call`starvote.reference.monkey_patch()`.  This does
+three things:
+
+* Adds the function to the `starvote` module directly,
+  as `starvote.allocated_score_voting_reference`.
+* Adds it to `starvote.__all__` so that symbol
+  gets brought in by `from starvote import *`.
+*
+* Adds the appropriate `Method` object
+  to `starvote.methods`, using the name
+  `'Allocated Score Voting (reference)'`
+  and the nickname `allocated_r`.
 
 *Note:* the reference implementation doesn't support
-tiebreakers.  `allocated_score_voting_reference` does
+tiebreakers.  `allocated_score_voting_reference` *does*
 accept a `tiebreaker` argument, but currently it *must*
 be `None`.
 
 ### Ties
 
 The good news is, STAR Voting elections rarely result in a tie in the
 real world.  But ties can still happen.  The good news is, STAR Voting
@@ -738,15 +754,15 @@
 
 You can experiment with these with the command-line version of the
 module, too.  You can specify the electoral system with `-e`,
 the number of seats with `-s`,
 and the maximum score with `-m`:
 
 ```
-% python3 -m starvote -e Reweighted_Range -s 3 -m 10 sample_polls/sample_poll_reweighted_range_3_seats.csv
+% python3 -m starvote test_elections/test_election_reweighted_range_sample_election.starvote
 ```
 
 ### Warning
 
 I haven't found a single test corpus for Bloc STAR Voting.
 I'm following the rules as best I can, and the results I'm getting
 make sense.  But so far I can't confirm my implementation is
@@ -788,14 +804,30 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.3** - *2023/05/27*
+
+* Normalized nomenclature for `Method` objects.  Now,
+  every method has an official correctly-spelled
+  correctly-capitalized name, and exactly one "nickname".
+  The nickname is always lowercase, and would return
+  True for `isidentifier`.  These are used in the
+  `starvote.method` map; a variant of these names is
+  also bound as module attributes (changed so they're
+  valid identifiers).
+* Improved `starvote.reference.monkey_patch`.  It's now
+  data-driven and thus more reliable.
+* Added `starvote.reference.__all__`, in case you want
+  to `from starvote.reference import *`.
+* Doc fixes.
+
 **2.0.2** - *2023/05/27*
 
 * Renamed the `tiebreaker` parameter `candidates` to `tie`.
 * Evicted some testing-only tiebreakers from the `starvote`
   module.  They're now in their own script, which only gets
   loaded when working with the test suite.
```

