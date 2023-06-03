# Comparing `tmp/starvote-2.0.1.tar.gz` & `tmp/starvote-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-2.0.1.tar` & `starvote-2.0.2.tar`

### file list

```diff
@@ -1,161 +1,162 @@
--rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.1/LICENSE
--rw-r--r--   0        0        0    32302 2023-06-02 20:05:55.863662 starvote-2.0.1/README.md
--rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.1/docs/clarifying_star_voting.md
--rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.1/docs/formatting_fractions_in_columns_of_text.txt
--rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.1/example.py
--rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    90423 2023-06-02 20:04:35.358964 starvote-2.0.1/starvote/__init__.py
--rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.1/starvote/__main__.py
--rw-r--r--   0        0        0     5781 2023-06-02 20:04:16.742802 starvote-2.0.1/starvote/reference.py
--rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.1/test_elections/README.md
--rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.1/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
--rw-r--r--   0        0        0     1358 2023-06-02 19:23:34.765586 starvote-2.0.1/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.1/test_elections/bad_syntax_change_section_in_list.starvote
--rw-r--r--   0        0        0     1395 2023-06-02 19:23:34.765586 starvote-2.0.1/test_elections/bad_syntax_change_section_in_list.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
--rw-r--r--   0        0        0     1404 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
--rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
--rw-r--r--   0        0        0     1402 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
--rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.1/test_elections/bad_syntax_invalid_method.starvote
--rw-r--r--   0        0        0     1375 2023-06-02 19:31:54.613947 starvote-2.0.1/test_elections/bad_syntax_invalid_method.txt
--rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.1/test_elections/bad_syntax_invalid_option.starvote
--rw-r--r--   0        0        0     1374 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_option.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.1/test_elections/bad_syntax_invalid_pragma.starvote
--rw-r--r--   0        0        0     1376 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_pragma.txt
--rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.1/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
--rw-r--r--   0        0        0     1335 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_start_of_line_mode.txt
--rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_1.starvote
--rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_1.txt
--rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_2.starvote
--rw-r--r--   0        0        0     1360 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_2.txt
--rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.1/test_elections/bad_syntax_invalid_tiebreaker.starvote
--rw-r--r--   0        0        0     1382 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_tiebreaker.txt
--rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.1/test_elections/bad_syntax_malformed_section.starvote
--rw-r--r--   0        0        0     1371 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_malformed_section.txt
--rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.1/test_elections/bad_syntax_no_ballots.starvote
--rw-r--r--   0        0        0     1314 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_ballots.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.1/test_elections/bad_syntax_no_equals.starvote
--rw-r--r--   0        0        0     1346 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_equals.txt
--rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.1/test_elections/bad_syntax_no_method.starvote
--rw-r--r--   0        0        0     1409 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_method.txt
--rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.1/test_elections/bad_syntax_no_section.starvote
--rw-r--r--   0        0        0     1364 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_section.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.1/test_elections/bad_syntax_pragma_in_options.starvote
--rw-r--r--   0        0        0     1375 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_pragma_in_options.txt
--rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.1/test_elections/bad_syntax_pragma_inside_list.starvote
--rw-r--r--   0        0        0     1387 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_pragma_inside_list.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.1/test_elections/bad_syntax_repeated_option.starvote
--rw-r--r--   0        0        0     1380 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_repeated_option.txt
--rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.1/test_elections/bad_syntax_repeated_section.starvote
--rw-r--r--   0        0        0     1383 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_repeated_section.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
--rw-r--r--   0        0        0     1403 2023-06-02 19:23:34.773586 starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
--rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
--rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
--rw-r--r--   0        0        0     3193 2023-06-02 19:23:34.785586 starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.pdf
--rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.789586 starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
--rw-r--r--   0        0        0     2879 2023-06-02 19:23:34.789586 starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
--rw-r--r--   0        0        0     1596 2023-06-02 19:23:34.809586 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
--rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
--rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.117589 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
--rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
--rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.429592 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.pdf
--rw-r--r--   0        0        0      814 2023-06-02 19:23:35.433591 starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
--rw-r--r--   0        0        0      799 2023-06-02 19:23:35.433591 starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
--rw-r--r--   0        0        0     1434 2023-06-02 19:23:35.441592 starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
--rw-r--r--   0        0        0      747 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.1/test_elections/test_election_all_fives_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.1/test_elections/test_election_all_fives_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.1/test_elections/test_election_all_fives_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.1/test_elections/test_election_all_fives_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.1/test_elections/test_election_all_threes_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_threes_bloc_star.txt
--rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.1/test_elections/test_election_all_threes_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_threes_rrv.txt
--rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.1/test_elections/test_election_all_threes_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_threes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.1/test_elections/test_election_all_threes_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_threes_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.1/test_elections/test_election_all_zeroes_bloc_star.starvote
--rw-r--r--   0        0        0     1077 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.1/test_elections/test_election_all_zeroes_rrv.starvote
--rw-r--r--   0        0        0      481 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.1/test_elections/test_election_all_zeroes_star-pr.starvote
--rw-r--r--   0        0        0      473 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.1/test_elections/test_election_all_zeroes_star.starvote
--rw-r--r--   0        0        0     1027 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_star.txt
--rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.starvote
--rw-r--r--   0        0        0     3383 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.txt
--rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
--rw-r--r--   0        0        0     1606 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
--rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.1/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      831 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
--rw-r--r--   0        0        0      965 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
--rw-r--r--   0        0        0      744 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
--rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.starvote
--rw-r--r--   0        0        0      542 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.txt
--rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.starvote
--rw-r--r--   0        0        0     1087 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.txt
--rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.1/test_elections/test_election_extra_candidates_in_permutation.starvote
--rw-r--r--   0        0        0      142 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_extra_candidates_in_permutation.txt
--rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.1/test_elections/test_election_incomplete_permutation.starvote
--rw-r--r--   0        0        0      138 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_incomplete_permutation.txt
--rw-r--r--   0        0        0      132 2023-06-02 01:44:01.610291 starvote-2.0.1/test_elections/test_election_no_output.starvote
--rw-r--r--   0        0        0       17 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_no_output.txt
--rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.1/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
--rw-r--r--   0        0        0     1329 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
--rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.1/test_elections/test_election_only_one_candidate_star.starvote
--rw-r--r--   0        0        0      505 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_one_candidate_star.txt
--rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.1/test_elections/test_election_only_two_candidates_bloc_star.starvote
--rw-r--r--   0        0        0      487 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_two_candidates_bloc_star.txt
--rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.1/test_elections/test_election_only_two_candidates_rrv.starvote
--rw-r--r--   0        0        0      523 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_two_candidates_rrv.txt
--rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.1/test_elections/test_election_only_two_candidates_star-pr.starvote
--rw-r--r--   0        0        0      545 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_two_candidates_star-pr.txt
--rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.1/test_elections/test_election_proportional_star_unbreakable_tie.starvote
--rw-r--r--   0        0        0      480 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_proportional_star_unbreakable_tie.txt
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.html
--rw-r--r--   0        0        0      450 2023-05-31 14:05:31.788268 starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.starvote
--rw-r--r--   0        0        0     1150 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
--rw-r--r--   0        0        0     1023 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
--rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0     1788 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
--rw-r--r--   0        0        0     2029 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.1/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      938 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.1/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
--rw-r--r--   0        0        0     1081 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
--rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.1/test_elections/test_election_use_just_raise_tiebreaker.starvote
--rw-r--r--   0        0        0     1197 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_use_just_raise_tiebreaker.txt
--rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.1/test_elections/test_election_use_no_description_tiebreaker.starvote
--rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_use_no_description_tiebreaker.txt
--rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.1/test_elections/test_election_use_only_heading_tiebreaker.starvote
--rw-r--r--   0        0        0      152 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_use_only_heading_tiebreaker.txt
--rw-r--r--   0        0        0    35726 2023-06-02 19:26:39.999204 starvote-2.0.1/tests/run_tests.py
--rwxr-xr-x   0        0        0     2211 2023-06-02 19:34:15.379168 starvote-2.0.1/tools/is_ok
--rwxr-xr-x   0        0        0     1827 2023-06-02 18:03:13.135277 starvote-2.0.1/tools/remake_test_elections_output
--rw-r--r--   0        0        0    32872 1970-01-01 00:00:00.000000 starvote-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.2/LICENSE
+-rw-r--r--   0        0        0    33924 2023-06-03 00:28:40.930575 starvote-2.0.2/README.md
+-rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.2/docs/clarifying_star_voting.md
+-rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.2/docs/formatting_fractions_in_columns_of_text.txt
+-rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.2/example.py
+-rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    89901 2023-06-03 00:25:56.353104 starvote-2.0.2/starvote/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.2/starvote/__main__.py
+-rw-r--r--   0        0        0     5781 2023-06-02 20:04:16.742802 starvote-2.0.2/starvote/reference.py
+-rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.2/test_elections/README.md
+-rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.2/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
+-rw-r--r--   0        0        0     1358 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.2/test_elections/bad_syntax_change_section_in_list.starvote
+-rw-r--r--   0        0        0     1395 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_change_section_in_list.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
+-rw-r--r--   0        0        0     1404 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
+-rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
+-rw-r--r--   0        0        0     1402 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
+-rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.2/test_elections/bad_syntax_invalid_method.starvote
+-rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_method.txt
+-rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.2/test_elections/bad_syntax_invalid_option.starvote
+-rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_option.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.2/test_elections/bad_syntax_invalid_pragma.starvote
+-rw-r--r--   0        0        0     1376 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_pragma.txt
+-rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.2/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
+-rw-r--r--   0        0        0     1335 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_start_of_line_mode.txt
+-rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_1.starvote
+-rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_1.txt
+-rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_2.starvote
+-rw-r--r--   0        0        0     1360 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_2.txt
+-rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.2/test_elections/bad_syntax_invalid_tiebreaker.starvote
+-rw-r--r--   0        0        0     1382 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_invalid_tiebreaker.txt
+-rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.2/test_elections/bad_syntax_malformed_section.starvote
+-rw-r--r--   0        0        0     1371 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_malformed_section.txt
+-rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.2/test_elections/bad_syntax_no_ballots.starvote
+-rw-r--r--   0        0        0     1314 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_ballots.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.2/test_elections/bad_syntax_no_equals.starvote
+-rw-r--r--   0        0        0     1346 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_equals.txt
+-rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.2/test_elections/bad_syntax_no_method.starvote
+-rw-r--r--   0        0        0     1409 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_method.txt
+-rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.2/test_elections/bad_syntax_no_section.starvote
+-rw-r--r--   0        0        0     1364 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_no_section.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.2/test_elections/bad_syntax_pragma_in_options.starvote
+-rw-r--r--   0        0        0     1375 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_pragma_in_options.txt
+-rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.2/test_elections/bad_syntax_pragma_inside_list.starvote
+-rw-r--r--   0        0        0     1387 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_pragma_inside_list.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.2/test_elections/bad_syntax_repeated_option.starvote
+-rw-r--r--   0        0        0     1380 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_repeated_option.txt
+-rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.2/test_elections/bad_syntax_repeated_section.starvote
+-rw-r--r--   0        0        0     1383 2023-06-03 00:24:26.568301 starvote-2.0.2/test_elections/bad_syntax_repeated_section.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
+-rw-r--r--   0        0        0     1403 2023-06-03 00:24:26.576301 starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
+-rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
+-rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
+-rw-r--r--   0        0        0     3193 2023-06-03 00:24:26.584301 starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.pdf
+-rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.588301 starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
+-rw-r--r--   0        0        0     2879 2023-06-03 00:24:26.592301 starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
+-rw-r--r--   0        0        0     1596 2023-06-03 00:24:26.612301 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
+-rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
+-rw-r--r--   0        0        0    12586 2023-06-03 00:24:26.932304 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
+-rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
+-rw-r--r--   0        0        0    12586 2023-06-03 00:24:27.260307 starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.pdf
+-rw-r--r--   0        0        0      814 2023-06-03 00:24:27.264307 starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
+-rw-r--r--   0        0        0      799 2023-06-03 00:24:27.264307 starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
+-rw-r--r--   0        0        0     1434 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
+-rw-r--r--   0        0        0      747 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.2/test_elections/test_election_all_fives_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/test_election_all_fives_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.2/test_elections/test_election_all_fives_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-03 00:24:27.276307 starvote-2.0.2/test_elections/test_election_all_fives_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.2/test_elections/test_election_all_fives_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_fives_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.2/test_elections/test_election_all_fives_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_fives_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.2/test_elections/test_election_all_threes_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_bloc_star.txt
+-rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.2/test_elections/test_election_all_threes_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_rrv.txt
+-rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.2/test_elections/test_election_all_threes_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.2/test_elections/test_election_all_threes_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_threes_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.2/test_elections/test_election_all_zeroes_bloc_star.starvote
+-rw-r--r--   0        0        0     1077 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.2/test_elections/test_election_all_zeroes_rrv.starvote
+-rw-r--r--   0        0        0      481 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.2/test_elections/test_election_all_zeroes_star-pr.starvote
+-rw-r--r--   0        0        0      473 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.2/test_elections/test_election_all_zeroes_star.starvote
+-rw-r--r--   0        0        0     1027 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_all_zeroes_star.txt
+-rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.starvote
+-rw-r--r--   0        0        0     3383 2023-06-03 00:24:27.280307 starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.txt
+-rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
+-rw-r--r--   0        0        0     1606 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
+-rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.2/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      831 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
+-rw-r--r--   0        0        0      965 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
+-rw-r--r--   0        0        0      744 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
+-rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.starvote
+-rw-r--r--   0        0        0      542 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.txt
+-rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.starvote
+-rw-r--r--   0        0        0     1087 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.txt
+-rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.2/test_elections/test_election_extra_candidates_in_permutation.starvote
+-rw-r--r--   0        0        0      142 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_extra_candidates_in_permutation.txt
+-rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.2/test_elections/test_election_incomplete_permutation.starvote
+-rw-r--r--   0        0        0      138 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_incomplete_permutation.txt
+-rw-r--r--   0        0        0      132 2023-06-02 01:44:01.610291 starvote-2.0.2/test_elections/test_election_no_output.starvote
+-rw-r--r--   0        0        0       17 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_no_output.txt
+-rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.2/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
+-rw-r--r--   0        0        0     1329 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
+-rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.2/test_elections/test_election_only_one_candidate_star.starvote
+-rw-r--r--   0        0        0      505 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_one_candidate_star.txt
+-rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.2/test_elections/test_election_only_two_candidates_bloc_star.starvote
+-rw-r--r--   0        0        0      487 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_two_candidates_bloc_star.txt
+-rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.2/test_elections/test_election_only_two_candidates_rrv.starvote
+-rw-r--r--   0        0        0      523 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_two_candidates_rrv.txt
+-rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.2/test_elections/test_election_only_two_candidates_star-pr.starvote
+-rw-r--r--   0        0        0      545 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_only_two_candidates_star-pr.txt
+-rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.2/test_elections/test_election_proportional_star_unbreakable_tie.starvote
+-rw-r--r--   0        0        0      480 2023-06-03 00:24:27.284307 starvote-2.0.2/test_elections/test_election_proportional_star_unbreakable_tie.txt
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.html
+-rw-r--r--   0        0        0      450 2023-05-31 14:05:31.788268 starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.starvote
+-rw-r--r--   0        0        0     1150 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
+-rw-r--r--   0        0        0     1023 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
+-rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0     1788 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
+-rw-r--r--   0        0        0     2029 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.2/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      938 2023-06-03 00:24:27.288307 starvote-2.0.2/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.2/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
+-rw-r--r--   0        0        0     1081 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
+-rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.2/test_elections/test_election_use_just_raise_tiebreaker.starvote
+-rw-r--r--   0        0        0     1103 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_use_just_raise_tiebreaker.txt
+-rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.2/test_elections/test_election_use_no_description_tiebreaker.starvote
+-rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_use_no_description_tiebreaker.txt
+-rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.2/test_elections/test_election_use_only_heading_tiebreaker.starvote
+-rw-r--r--   0        0        0      152 2023-06-03 00:24:27.292307 starvote-2.0.2/test_elections/test_election_use_only_heading_tiebreaker.txt
+-rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.2/tests/harness.py
+-rw-r--r--   0        0        0    35844 2023-06-03 00:26:24.333354 starvote-2.0.2/tests/run_tests.py
+-rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.2/tools/is_ok
+-rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.2/tools/remake_test_elections_output
+-rw-r--r--   0        0        0    34494 1970-01-01 00:00:00.000000 starvote-2.0.2/PKG-INFO
```

### Comparing `starvote-2.0.1/LICENSE` & `starvote-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/README.md` & `starvote-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -176,130 +176,176 @@
     maximum_score=5,
     print=None,
     seats=1,
     verbosity=0,
     ):
 ```
 
+`election` tabulates an election based on your
+parameter and returns a `list` containing the
+winners. (Even for single-winner STAR Voting--in
+that case, the list will only contain one element.)
+
 `method` specifies which election system you want to use.
 The allowed values are
-`starvote.STAR`,
-`starvote.Bloc_STAR`,
-`starvote.Proportional_STAR`,
+`starvote.STAR_Voting`,
+`starvote.Bloc_STAR_Voting`,
+`starvote.Allocated_Score_Voting`,
 and
-`starvote.Reweighted_Range`.
+`starvote.Reweighted_Range_Voting`.  (Since those are a lot to
+type, `starvote` also provides nicknames, respectively:
+`starvote.star`, `starvote.bloc`, `starvote.allocated`,
+and `starvote.rrv`.)
 
 `ballots` should be an iterable containing individual ballots.
 Ballots are `dict` objects, mapping the candidate to that ballot's
 score for that candidate.  The candidate can be any Python value;
 the score must be an `int`.
 
 `maximum_score` specifies the maximum score allowed for any vote
 on any ballot.
 
 `seats` specifies how many seats the election should fill.
-STAR Voting is a single-winner method, so this should be 1 when
-using STAR Voting; for all the other methods,
-`seats` must be greater than or equal to 2.
+STAR Voting is a single-winner method, so this should be
+`1` when using STAR Voting; for all the other methods,
+`seats` must be greater than or equal to `2`.
 
 `verbosity` specifies how much output you want.
-The default of 0 suppresses input; `verbosity=1` produces
-human-readable output, and `verbosity=2` adds some additional
-information (the "preferences matrix" for STAR runoff rounds).
-
-`print` lets you specify your own printing function.  By default
-`election` will use `builtins.print`; your replacement `print`
-function should have the same signature.
-
-`election` tabulates the election and returns a list of the winners.
-(Even for single-winner STAR Voting--in that case, the list will
-only contain one element.)
+The current supported values are `0` (no output)
+and `1` (output); values higher than `1` are
+currently equivalent to `1`.
+
+`print` lets you specify your own printing function.
+By default `election` will use `builtins.print`;
+your replacement `print` function should have the
+same signature.
+
 
 
 ### Functions for specific electoral systems
 
-`starvote` also exports functions that implement each of
+`starvote` also exports functions implementing each of
 the supported electoral systems:
 
 * `star_voting` implements single-winner STAR Voting.
 * `bloc_star_voting` implements multi-winner Bloc STAR Voting.
 * `allocated_score_voting` implements Allocated Score Voting.
-* `reweighted_range` implements Reweighted Range Voting.
+* `reweighted_range_voting` implements Reweighted Range Voting.
 
 These functions take much the same signature as `election`,
 with the following changes:
 
 * They don't take the `method` positional parameter;
   the method is implicit in the function.  All four only
   take one positional parameter, `ballots`, which is
   required.
 * `star` doesn't take a `seats` parameter.  The other three
   have a `seats` keyword-only parameter, and this parameter
   is required--it doesn't have a default.  (A required
   keyword-only parameter is pretty rare in Python!)
 * Note that these functions also always return a list,
-  including `star`.
+  even `star_voting`.
 
 #### Reference implementation of Allocated Score Voting
 
-`starvote` also ships a copy of the reference implementation
-of Allocated Score Voting.  This requires both NumPy and Pandas,
-so it's not imported by default.  (I didn't want `starvote`
-to have any external dependencies.  The unit test suite runs
-correctly whether or not these external dependencies are installed.)
-
-You can import it with `import starvote.reference`, and you can
-integrate it into the `starvote` module by calling
-`starvote.reference.monkey_patch()`.  Its implementation
-function can be found at
+`starvote` ships a copy of the reference implementation
+of Allocated Score Voting.  Since this requires both NumPy
+and Pandas, it's not imported by default.  (I didn't want
+`starvote` to have any external dependencies.  The unit
+test suite runs correctly whether or not these external
+dependencies are installed.)
+
+You can import it with `import starvote.reference`,
+and you can integrate it into the `starvote` module by
+calling `starvote.reference.monkey_patch()`.  Its
+implementation function can be found at
 `starvote.reference.allocated_score_voting_reference`,
 and it's added to `methods` under the name
 `'Allocated Score Voting (reference)'`.
 
-*Note:* the reference implementation doesn't support tiebreakers.
-`tiebreaker` must be `None`.
+*Note:* the reference implementation doesn't support
+tiebreakers.  `allocated_score_voting_reference` does
+accept a `tiebreaker` argument, but currently it *must*
+be `None`.
 
 ### Ties
 
 The good news is, STAR Voting elections rarely result in a tie in the
 real world.  But ties can still happen.  The good news is, STAR Voting
 has a sensible, thorough protocol on how to break a tie.  The bad news is,
 not all ties are breakable--some ties genuinely represent the ambivalent
 will of the voters.
 
 **starvote** gives you control over how to break ties in elections,
 through the `tiebreaker` parameter to `election` and the election-specific
 functions.  **starvote** also has two predefined tiebreaker functions,
 but you can substitute your own--or none at all.
 
+The default tiebreaker in **starvote** is
+`predefined_permutation_tiebreaker`, passing
+in `candidates=None`.
+
 #### `predefined_permutation_tiebreaker`
 
 The main tiebreaker for **starvote** is
 `predefined_permutation_tiebreaker`.  This
+is a class; you should instantiate it and
+pass in the instance as the `tiebreaker`
+argument when you run the election.
+
+`predefined_permutation_tiebreaker`
 resolves the tie in favor of an ordered
-list of candidates--the candidate(s) that
-appear earliest in the list win the tie.
+list of candidates.
 
-If you don't pass in a list of candidates,
-`predefined_permutation_tiebreaker` will scan
-the ballots at the start of the election to
-produce a list of all the candidates, then
-randomly shuffle the list and use *that* list
-as the list of candidates.
-
-`predefined_permutation_tiebreaker` prints
-the permuted list of candidates at election
-initialization time, and prints its process
+Given these three variables, defined
+at the time it breaks the tie:
+
+* `candidates`, an ordered list of *all*
+  candidates participating in the election,
+* `tie`, an iterable of the tied candidates, and
+* `desired`, the number of winners we wanted.
+
+`predefined_permutation_tiebreaker` computes
+the winners of the tie as follows:
+
+```
+winners = [c for c in candidates if c in tie][:desired]
+```
+
+In other words, it returns a *desired*-length
+subset of *tie*, preferring candidates that
+appear earlier in *candidates* over those that
+appear later.
+
+`predefined_permutation_tiebreaker` accepts
+a `candidates` argument, which should be
+an ordered pre-chosen list of all candidates.
+The default value is `None`, which instructs
+`predefined_permutation_tiebreaker` to scan
+the ballots at the start of the election,
+produce its own list of all the candidates,
+randomly shuffle that list, and use that list
+as the `candidates` list.
+
+If you pass in your own `candidates` list,
+you may also pass in a string for the
+`description` keyword-only parameter, which
+should be text describing the source of
+this ordered list of candidates.
 
 #### `on_demand_random_tiebreaker`
 
-If you prefer you can use `on_demand_random_tiebreaker`
+If you prefer more unpredictability in your life,
+you can choose `on_demand_random_tiebreaker`
 to break ties.  `on_demand_random_tiebreaker` will
 simply pick a random candidate (or candidates)
 on demand, using Python's `random.sample` function.
+`on_demand_random_tiebreaker` is a function;
+you should simply pass it in as the `tiebreaker`
+parameter.
 
 #### `UnbreakableTieError`
 
 If you explicitly set `tiebreaker` to `None`,
 and an election results in a tie, `starvote` will
 raise an `UnbreakableTieError` exception.  You can
 get a text description of the tie by calling `str` on the exception;
@@ -312,15 +358,15 @@
 in the `tiebreaker` parameter to your chosen election
 function.  Custom tiebreakers can be either a function
 or a class.
 
 A custom tiebreaker function should have this signature:
 
 ```Python
-def custom_tiebreaker(options, candidates, desired, exception):
+def custom_tiebreaker(options, tie, desired, exception):
 ```
 
 Here's what these four parameters will contain:
 
 * `options` is a **starvote** `Options` object.  `options`
   has attributes mapping to the arguments you passed in to
   `election`.  You should obey `options.verbosity` when
@@ -337,27 +383,28 @@
     first (and only) positional argument.  Also accepts
     a `numbered` parameter; if `numbered` is true, it
     prints the candidates in order, prepended by their
     ordinal number (starting with 1).  If `numbered` is
     false, `print_candidates` attempts to sort the
     candidates before printing them.
 
-* `candidates` is a list of the tied candidates.
+* `tie` is a list of the tied candidates.
 
 * `desired` is the desired number of winners.
 
 * `exception` is the `UnbreakableTieError` for this
   tie.  If you can't break the tie, you should raise
   this object.
 
-Note that **starvote** will parse the tiebreaker function's
-docstring.  The first line of the docstring will be used
-as a "heading" printed during election initialization, with
-the rest of the docstring printed as the body of that heading
-if `options.verbosity` is 1 or greater.
+Note that **starvote** will also parse the tiebreaker
+function's docstring.  The first line of the docstring
+will be used as a "heading" printed during election
+initialization, with the rest of the docstring will be
+printed as the body of that heading if `options.verbosity`
+is 1 or greater.
 
 You can also write a custom tiebreaker class.  The only
 requirement is that the class inherits from
 `starvote.Tiebreaker`, and it supports a `__call__` method
 with the same signature as a custom tiebreaker function.
 (However, here the docstring is ignored; it's up to you
 to call `options.heading` and `options.print`.)
@@ -405,37 +452,37 @@
 Git repo.)
 
 After this example code finishes,
 the `winners` variable will contain the list `['Chuck']`.
 The example also produces this output:
 
 ```
-[STAR]
+[STAR Voting]
   Tabulating 3 ballots.
   Maximum score is 5.
-[STAR: Initializing ordered permutation tiebreaker]
+[STAR Voting: Initializing ordered permutation tiebreaker]
   Computing a random permutation of all the candidates.
   Permuted list of candidates:
-    1. Chuck
-    2. Amy
-    3. Brian
+    1. Brian
+    2. Chuck
+    3. Amy
   Tiebreaker candidates will be selected from this list, preferring candidates with lower numbers.
-[STAR: Scoring Round]
+[STAR Voting: Scoring Round]
   The two highest-scoring candidates advance to the next round.
     Chuck -- 13 (average 4+1/3) -- First place
     Amy   -- 10 (average 3+1/3) -- Second place
     Brian --  9 (average 3)
   Chuck and Amy advance.
-[STAR: Automatic Runoff Round]
+[STAR Voting: Automatic Runoff Round]
   The candidate preferred in the most head-to-head matchups wins.
     Chuck         -- 2 -- First place
     Amy           -- 1
     No Preference -- 0
   Chuck wins.
-[STAR: Winner]
+[STAR Voting: Winner]
   Chuck
 ```
 
 
 ### *starvote format*
 
 `starvote` also defines a custom text format for specifying
@@ -726,14 +773,21 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.2** - *2023/05/27*
+
+* Renamed the `tiebreaker` parameter `candidates` to `tie`.
+* Evicted some testing-only tiebreakers from the `starvote`
+  module.  They're now in their own script, which only gets
+  loaded when working with the test suite.
+
 **2.0.1** - *2023/05/27*
 
 * Changed the nickname of the reference version of
   Allocated Score Voting to "Allocated-R".
 
 **2.0** - *2023/05/27*
```

### Comparing `starvote-2.0.1/docs/clarifying_star_voting.md` & `starvote-2.0.2/docs/clarifying_star_voting.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/docs/formatting_fractions_in_columns_of_text.txt` & `starvote-2.0.2/docs/formatting_fractions_in_columns_of_text.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/pyproject.toml` & `starvote-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/starvote/__init__.py` & `starvote-2.0.2/starvote/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 #!/usr/bin/env python3
 
+##
+## TODO
+##
+## * write a unit test that confirms "example.py"
+##   runs, and the output in README.md is up to date
+##   (I keep breaking it / its output keeps getting outdated.)
+##
+
 __doc__ = "An election tabulator for the STAR electoral system, and others"
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 __all__ = [
     'Allocated_Score_Voting', # Method
     'Allocated', # Method (nickname)
     'allocated_score_voting', # function
     'Bloc_STAR_Voting', # Method
     'Bloc', # Method (nickname)
@@ -216,15 +224,15 @@
         self.desired = desired
 
 
 class Tiebreaker:
     def initialize(self, options, ballots): # pragma: no cover
         pass
 
-    def __call__(self, options, candidates, desired, exception): # pragma: no cover
+    def __call__(self, options, tie, desired, exception): # pragma: no cover
         pass
 
     def print_description(self, options, description):
         if not description: # pragma: no cover
             return
         if isinstance(description, str):
             options.print(description)
@@ -256,71 +264,43 @@
         return f"TiebreakerFunctionWrapper(function={self.function})"
 
     def initialize(self, options, ballots):
         if self.heading:
             with options.heading(self.heading):
                 self.print_description(options, self.description)
 
-    def __call__(self, options, candidates, desired, exception):
-        return self.function(options, candidates, desired, exception)
+    def __call__(self, options, tie, desired, exception):
+        return self.function(options, tie, desired, exception)
 
 
 tiebreakers = {'None': None, 'none': None}
 
 def _add_tiebreaker(o):
     tiebreakers[o.__name__] = o
     return o
 
 @_add_tiebreaker
-def on_demand_random_tiebreaker(options, candidates, desired, exception):
+def on_demand_random_tiebreaker(options, tie, desired, exception):
     """
     On-demand random tiebreaker
 
     Tie-breaking winners will be chosen at random, on demand.
     """
-    result = random.sample(population=candidates, k=desired)
+    result = random.sample(population=tie, k=desired)
     with options.heading("On-demand random tiebreaker"):
         if options.verbosity:
             two_candidates = "two candidates" if desired == 2 else "one candidate"
             options.print(f"Choosing {two_candidates} from this list:")
-            options.print_candidates(candidates)
+            options.print_candidates(tie)
             if desired == 1:
                 options.print(f"Randomly chose winner: {result[0]}")
             else:
                 options.print(f"Randomly chose winners: {' and '.join(result)}")
     return result
 
-@_add_tiebreaker
-def _just_raise_tiebreaker(options, candidates, desired, exception):
-    """
-    Just raise tiebreaker
-
-
-    Raises the exception immediately.
-    Don't actually use this, it's pointless.
-    It's only useful for coverage in the test suite.
-
-
-    """
-    raise exception
-
-@_add_tiebreaker
-def _only_heading_tiebreaker(options, candidates, desired, exception): # pragma: nocover
-    """
-    This tiebreaker only has a heading, no description.
-
-
-    """
-    raise exception
-
-@_add_tiebreaker
-def _no_description_tiebreaker(options, candidates, desired, exception):
-    # don't use this, it's only for testing
-    raise exception
-
 
 @_add_tiebreaker
 class predefined_permutation_tiebreaker(Tiebreaker):
     def __init__(self, candidates=None, *, description=None):
         if (not candidates) and description:
             raise ValueError("you can't specify a message unless you specify an iterable of candidates")
         self.candidates = candidates
@@ -364,22 +344,22 @@
         if options.verbosity:
             with options.heading("Initializing ordered permutation tiebreaker"):
                 self.print_description(options, self.description)
                 options.print("Permuted list of candidates:")
                 options.print_candidates(self.candidates, numbered=True)
                 options.print("Tiebreaker candidates will be selected from this list, preferring candidates with lower numbers.")
 
-    def __call__(self, options, candidates, desired, exception):
-        subset = set(candidates)
-        result = [candidate for candidate in self.candidates if candidate in subset][:desired]
+    def __call__(self, options, tie, desired, exception):
+        tie_set = set(tie)
+        result = [candidate for candidate in self.candidates if candidate in tie_set][:desired]
         if options.verbosity:
             with options.heading("Predefined permutation tiebreaker"):
                 two = "two " if desired == 2 else ""
                 options.print(f"Choosing the earliest {two}of these candidates from the permuted list:")
-                options.print_candidates(candidates)
+                options.print_candidates(tie)
                 if desired == 1:
                     options.print(f"Selected winner: {result[0]}")
                 else:
                     options.print(f"Selected winners: {' and '.join(result)}")
         return result
```

### Comparing `starvote-2.0.1/starvote/reference.py` & `starvote-2.0.2/starvote/reference.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/README.md` & `starvote-2.0.2/test_elections/README.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_ballot_pragma_as_last_line.txt` & `starvote-2.0.2/test_elections/bad_syntax_ballot_pragma_as_last_line.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_change_section_in_list.txt` & `starvote-2.0.2/test_elections/bad_syntax_change_section_in_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_1.txt` & `starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_2.txt` & `starvote-2.0.2/test_elections/bad_syntax_fussy_wrong_ballots_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_method.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_method.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
 
 ballots_file should be a path to a file ending either in '.csv' or '.star':
 
     * .csv files must be in https://start.vote CSV format.
       When loading a .csv file, starvote defaults to STAR Voting,
       one seat, verbosity 1, and
     * .starvote files must be in "starvote format".
-
```

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_option.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_pragma.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_pragma.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_start_of_line_mode.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_start_of_line_mode.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_1.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_2.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_starvote_path_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_invalid_tiebreaker.txt` & `starvote-2.0.2/test_elections/bad_syntax_invalid_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_malformed_section.txt` & `starvote-2.0.2/test_elections/bad_syntax_malformed_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_no_ballots.txt` & `starvote-2.0.2/test_elections/bad_syntax_no_ballots.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_no_equals.txt` & `starvote-2.0.2/test_elections/bad_syntax_no_equals.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_no_method.txt` & `starvote-2.0.2/test_elections/bad_syntax_no_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_no_section.txt` & `starvote-2.0.2/test_elections/bad_syntax_no_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_pragma_in_options.txt` & `starvote-2.0.2/test_elections/bad_syntax_pragma_in_options.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_pragma_inside_list.txt` & `starvote-2.0.2/test_elections/bad_syntax_pragma_inside_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_repeated_option.txt` & `starvote-2.0.2/test_elections/bad_syntax_repeated_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/bad_syntax_repeated_section.txt` & `starvote-2.0.2/test_elections/bad_syntax_repeated_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt` & `starvote-2.0.2/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv` & `starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt` & `starvote-2.0.2/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.csv` & `starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.txt` & `starvote-2.0.2/test_elections/starvote_ballots_best_akali_skins.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.txt` & `starvote-2.0.2/test_elections/starvote_ballots_eurovision_song_contest_2023.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt` & `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt` & `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt` & `starvote-2.0.2/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.csv` & `starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.txt` & `starvote-2.0.2/test_elections/starvote_ballots_presidential_candidates.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.txt` & `starvote-2.0.2/test_elections/starvote_ballots_presidential_poll_july_2020.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt` & `starvote-2.0.2/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf` & `starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt` & `starvote-2.0.2/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_all_fives_bloc_star.txt` & `starvote-2.0.2/test_elections/test_election_all_fives_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_all_fives_star.txt` & `starvote-2.0.2/test_elections/test_election_all_fives_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_all_threes_bloc_star.txt` & `starvote-2.0.2/test_elections/test_election_all_threes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_all_threes_star.txt` & `starvote-2.0.2/test_elections/test_election_all_threes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_all_zeroes_bloc_star.txt` & `starvote-2.0.2/test_elections/test_election_all_zeroes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_all_zeroes_star.txt` & `starvote-2.0.2/test_elections/test_election_all_zeroes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.starvote` & `starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.txt` & `starvote-2.0.2/test_elections/test_election_bloc_star_and_electowiki.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote` & `starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt` & `starvote-2.0.2/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_breakable_tie_for_second_in_score_round.txt` & `starvote-2.0.2/test_elections/test_election_breakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt` & `starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt` & `starvote-2.0.2/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.starvote` & `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.txt` & `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.starvote` & `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.txt` & `starvote-2.0.2/test_elections/test_election_demonstrate_cloneproofness_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_no_permuted_candidates_tiebreaker.txt` & `starvote-2.0.2/test_elections/test_election_no_permuted_candidates_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_only_two_candidates_rrv.txt` & `starvote-2.0.2/test_elections/test_election_only_two_candidates_rrv.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_only_two_candidates_star-pr.txt` & `starvote-2.0.2/test_elections/test_election_only_two_candidates_star-pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.html` & `starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.html`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.txt` & `starvote-2.0.2/test_elections/test_election_reweighted_range_sample_election.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt` & `starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt` & `starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt` & `starvote-2.0.2/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt` & `starvote-2.0.2/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt` & `starvote-2.0.2/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/test_elections/test_election_use_just_raise_tiebreaker.txt` & `starvote-2.0.2/test_elections/test_election_use_just_raise_tiebreaker.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [STAR Voting]
   Tabulating 5 ballots.
   Maximum score is 5.
 [STAR Voting: Just raise tiebreaker]
   Raises the exception immediately.
-  Don't actually use this, it's pointless.
-  It's only useful for coverage in the test suite.
 [STAR Voting: Scoring Round]
   The two highest-scoring candidates advance to the next round.
     Amy   -- 15 (average 3) -- Tied for first place
     Brian -- 15 (average 3) -- Tied for first place
     Chuck -- 15 (average 3) -- Tied for first place
   There's a three-way tie for first.
 [STAR Voting: Scoring Round: First tiebreaker]
```

### Comparing `starvote-2.0.1/test_elections/test_election_use_no_description_tiebreaker.txt` & `starvote-2.0.2/test_elections/test_election_use_no_description_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.1/tests/run_tests.py` & `starvote-2.0.2/tests/run_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,35 @@
 import unittest
 
 def preload_local_starvote():
     """
     Pre-load the local "starvote" module, to preclude finding
     an already-installed one on the path.
     """
-    from os.path import abspath, dirname, isfile, join, normpath
     import sys
-    starvote_dir = abspath(dirname(sys.argv[0]))
+    import pathlib
+    argv_0 = pathlib.Path(sys.argv[0])
+    starvote_dir = argv_0.parent.resolve()
     while True:
-        starvote_init = join(starvote_dir, "starvote/__init__.py")
-        if isfile(starvote_init):
+        starvote_init = starvote_dir / "starvote" / "__init__.py"
+        if starvote_init.is_file():
             break
-        starvote_dir = normpath(join(starvote_dir, ".."))
-    sys.path.insert(1, starvote_dir)
+        starvote_dir = starvote_dir.parent
+    sys.path.insert(0, str(starvote_dir))
     import starvote
-    return pathlib.Path(starvote_dir)
+    return starvote_dir
 
 starvote_dir = preload_local_starvote()
 import starvote
 
+#
+# Useless testing-only tiebreakers
+#
 
+import harness
 
 def inject_test_elections(cls, argv): # pragma: no cover
     """
     Finds all the test_election/{*.starvote, *.csv} files,
     runs the elections within, and compares the results to
     the corresponding .txt file.
 
@@ -60,15 +65,15 @@
             # real versions so the diff is readable
             smush_and_lower = lambda l: "\n".join(l).replace(' ', '').replace('\t', '').lower()
             smushed_and_lowered_expected = smush_and_lower(expected)
             smushed_and_lowered_got = smush_and_lower(got)
 
             if smushed_and_lowered_expected != smushed_and_lowered_got: # pragma: no cover
                 self.maxDiff = 2**32
-                self.assertEqual("\n".join(expected), "\n".join(got))
+                self.assertEqual("\n".join(expected) + "\n", "\n".join(got) + "\n")
         return run_test
 
     work = []
 
     argv = sys.argv[1:]
 
     # check .starvote before .csv
@@ -223,19 +228,19 @@
         with self.assertRaises(TypeError):
             o.break_tie(text="foo", candidates=3.14159, desired=1)
         with self.assertRaises(ValueError):
             o.break_tie(text="foo", candidates=[], desired=1)
         with self.assertRaises(ValueError):
             o.break_tie(text="foo", candidates=['a', 'b'], desired=3)
 
-        o = starvote.Options(method=starvote.STAR_Voting, verbosity=1, tiebreaker=lambda options, candidates, desired, tie: 3.1415)
+        o = starvote.Options(method=starvote.STAR_Voting, verbosity=1, tiebreaker=lambda options, tie, desired, exception: 3.1415)
         with self.assertRaises(TypeError):
             o.break_tie(text="foo", candidates=['a', 'b'], desired=1)
 
-        o = starvote.Options(method=starvote.STAR_Voting, verbosity=1, tiebreaker=lambda options, candidates, desired, tie: ['a', 'b', 'c', 'd', 'e'])
+        o = starvote.Options(method=starvote.STAR_Voting, verbosity=1, tiebreaker=lambda options, tie, desired, exception: ['a', 'b', 'c', 'd', 'e'])
         with self.assertRaises(TypeError):
             o.break_tie(text="foo", candidates=['a', 'b'], desired=1)
 
     def test_method(self):
         def fake_method(): # pragma: no cover
             pass
 
@@ -1117,9 +1122,11 @@
             'four hundred fifty-one quintillion two hundred thirty-four quadrillion five hundred sixty-seven trillion eight hundred ninety billion one hundred twenty-three million four hundred fifty-six thousand seven hundred eighty-nine',
             'four hundred and fifty-one quintillion, two hundred and thirty-four quadrillion, five hundred and sixty-seven trillion, eight hundred and ninety billion, one hundred and twenty-three million, four hundred and fifty-six thousand, seven hundred and eighty-nine')
 
         test((10**75) + 1,
             '1000000000000000000000000000000000000000000000000000000000000000000000000001',
             '1000000000000000000000000000000000000000000000000000000000000000000000000001')
 
-inject_test_elections(StarvoteTests, sys.argv[1:])
-unittest.main()
+if __name__ == '__main__':
+    # is_ok imports this to get the test tiebreakers
+    inject_test_elections(StarvoteTests, sys.argv[1:])
+    unittest.main()
```

### Comparing `starvote-2.0.1/tools/is_ok` & `starvote-2.0.2/tools/is_ok`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 
 def preload_local_starvote():
     """
     Pre-load the local "starvote" module, to preclude finding
     an already-installed one on the path.
     """
-    from os.path import abspath, dirname, isfile, join, normpath
     import sys
-    starvote_dir = abspath(dirname(sys.argv[0]))
+    import pathlib
+    argv_0 = pathlib.Path(sys.argv[0])
+    starvote_dir = argv_0.parent.resolve()
     while True:
-        starvote_init = join(starvote_dir, "starvote/__init__.py")
-        if isfile(starvote_init):
+        starvote_init = starvote_dir / "starvote" / "__init__.py"
+        if starvote_init.is_file():
             break
-        starvote_dir = normpath(join(starvote_dir, ".."))
-    sys.path.insert(1, starvote_dir)
+        starvote_dir = starvote_dir.parent
+    sys.path.insert(0, str(starvote_dir))
     import starvote
     return starvote_dir
 
 starvote_dir = preload_local_starvote()
 import starvote
 
 argv = sys.argv[1:]
@@ -34,15 +35,24 @@
     print("    % python -m starvote on <basename(path)>{.starvote,.csv}")
     print("and overwrites <basename>.txt with the result.")
     print()
     print("Used to refresh the .txt output files for the unit test suite.")
     sys.exit(0)
 
 starting_dir = pathlib.Path(os.getcwd())
-starvote_dir = pathlib.Path(starvote_dir)
+
+
+# load test scaffolding stuff (e.g. custom tiebreakers)
+# from unit test suite.
+# we don't actually need the symbols from inside,
+# they monkey-patch themselves in.
+sys.path.insert(0, str(starvote_dir / "tests"))
+import harness
+
+
 
 @contextlib.contextmanager
 def pushd(d):
     old_dir = os.getcwd()
     os.chdir(d)
     yield old_dir
     os.chdir(old_dir)
```

### Comparing `starvote-2.0.1/tools/remake_test_elections_output` & `starvote-2.0.2/tools/remake_test_elections_output`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 #!/usr/bin/env python3
 
 import glob
-import os.path
+import os
+import pathlib
 import sys
 
+argv_0 = pathlib.Path(sys.argv[0])
+
 try:
     import pandas
     import numpy
 except ImportError:
-    print(f"{os.path.basename(sys.argv[0])} requires both Pandas and NumPy.")
+    print(f"{argv_0.name} requires both Pandas and NumPy.")
     print()
     print("Run this:")
     print(f"  % {sys.executable} -m pip install pandas numpy")
     sys.exit(-1)
 
 def preload_local_starvote():
     """
     Pre-load the local "starvote" module, to preclude finding
     an already-installed one on the path.
     """
-    from os.path import abspath, dirname, isfile, join, normpath
     import sys
-    starvote_dir = abspath(dirname(sys.argv[0]))
+    import pathlib
+    argv_0 = pathlib.Path(sys.argv[0])
+    starvote_dir = argv_0.parent.resolve()
     while True:
-        starvote_init = join(starvote_dir, "starvote/__init__.py")
-        if isfile(starvote_init):
+        starvote_init = starvote_dir / "starvote" / "__init__.py"
+        if starvote_init.is_file():
             break
-        starvote_dir = normpath(join(starvote_dir, ".."))
-    sys.path.insert(1, starvote_dir)
+        starvote_dir = starvote_dir.parent
+    sys.path.insert(0, str(starvote_dir))
     import starvote
     return starvote_dir
 
 starvote_dir = preload_local_starvote()
 import starvote.reference
 
 starvote.reference.monkey_patch()
 
+# load test scaffolding stuff (e.g. custom tiebreakers)
+# from unit test suite.
+# we don't actually need the symbols from inside,
+# they monkey-patch themselves in.
+sys.path.insert(0, str(starvote_dir / "tests"))
+import harness
+
+
 os.chdir(starvote_dir)
 
 
 text = []
 
 def text_clear():
     text.clear()
```

### Comparing `starvote-2.0.1/PKG-INFO` & `starvote-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 2.0.1
+Version: 2.0.2
 Summary: An election tabulator for the STAR electoral system, and others
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -191,130 +191,176 @@
     maximum_score=5,
     print=None,
     seats=1,
     verbosity=0,
     ):
 ```
 
+`election` tabulates an election based on your
+parameter and returns a `list` containing the
+winners. (Even for single-winner STAR Voting--in
+that case, the list will only contain one element.)
+
 `method` specifies which election system you want to use.
 The allowed values are
-`starvote.STAR`,
-`starvote.Bloc_STAR`,
-`starvote.Proportional_STAR`,
+`starvote.STAR_Voting`,
+`starvote.Bloc_STAR_Voting`,
+`starvote.Allocated_Score_Voting`,
 and
-`starvote.Reweighted_Range`.
+`starvote.Reweighted_Range_Voting`.  (Since those are a lot to
+type, `starvote` also provides nicknames, respectively:
+`starvote.star`, `starvote.bloc`, `starvote.allocated`,
+and `starvote.rrv`.)
 
 `ballots` should be an iterable containing individual ballots.
 Ballots are `dict` objects, mapping the candidate to that ballot's
 score for that candidate.  The candidate can be any Python value;
 the score must be an `int`.
 
 `maximum_score` specifies the maximum score allowed for any vote
 on any ballot.
 
 `seats` specifies how many seats the election should fill.
-STAR Voting is a single-winner method, so this should be 1 when
-using STAR Voting; for all the other methods,
-`seats` must be greater than or equal to 2.
+STAR Voting is a single-winner method, so this should be
+`1` when using STAR Voting; for all the other methods,
+`seats` must be greater than or equal to `2`.
 
 `verbosity` specifies how much output you want.
-The default of 0 suppresses input; `verbosity=1` produces
-human-readable output, and `verbosity=2` adds some additional
-information (the "preferences matrix" for STAR runoff rounds).
-
-`print` lets you specify your own printing function.  By default
-`election` will use `builtins.print`; your replacement `print`
-function should have the same signature.
-
-`election` tabulates the election and returns a list of the winners.
-(Even for single-winner STAR Voting--in that case, the list will
-only contain one element.)
+The current supported values are `0` (no output)
+and `1` (output); values higher than `1` are
+currently equivalent to `1`.
+
+`print` lets you specify your own printing function.
+By default `election` will use `builtins.print`;
+your replacement `print` function should have the
+same signature.
+
 
 
 ### Functions for specific electoral systems
 
-`starvote` also exports functions that implement each of
+`starvote` also exports functions implementing each of
 the supported electoral systems:
 
 * `star_voting` implements single-winner STAR Voting.
 * `bloc_star_voting` implements multi-winner Bloc STAR Voting.
 * `allocated_score_voting` implements Allocated Score Voting.
-* `reweighted_range` implements Reweighted Range Voting.
+* `reweighted_range_voting` implements Reweighted Range Voting.
 
 These functions take much the same signature as `election`,
 with the following changes:
 
 * They don't take the `method` positional parameter;
   the method is implicit in the function.  All four only
   take one positional parameter, `ballots`, which is
   required.
 * `star` doesn't take a `seats` parameter.  The other three
   have a `seats` keyword-only parameter, and this parameter
   is required--it doesn't have a default.  (A required
   keyword-only parameter is pretty rare in Python!)
 * Note that these functions also always return a list,
-  including `star`.
+  even `star_voting`.
 
 #### Reference implementation of Allocated Score Voting
 
-`starvote` also ships a copy of the reference implementation
-of Allocated Score Voting.  This requires both NumPy and Pandas,
-so it's not imported by default.  (I didn't want `starvote`
-to have any external dependencies.  The unit test suite runs
-correctly whether or not these external dependencies are installed.)
-
-You can import it with `import starvote.reference`, and you can
-integrate it into the `starvote` module by calling
-`starvote.reference.monkey_patch()`.  Its implementation
-function can be found at
+`starvote` ships a copy of the reference implementation
+of Allocated Score Voting.  Since this requires both NumPy
+and Pandas, it's not imported by default.  (I didn't want
+`starvote` to have any external dependencies.  The unit
+test suite runs correctly whether or not these external
+dependencies are installed.)
+
+You can import it with `import starvote.reference`,
+and you can integrate it into the `starvote` module by
+calling `starvote.reference.monkey_patch()`.  Its
+implementation function can be found at
 `starvote.reference.allocated_score_voting_reference`,
 and it's added to `methods` under the name
 `'Allocated Score Voting (reference)'`.
 
-*Note:* the reference implementation doesn't support tiebreakers.
-`tiebreaker` must be `None`.
+*Note:* the reference implementation doesn't support
+tiebreakers.  `allocated_score_voting_reference` does
+accept a `tiebreaker` argument, but currently it *must*
+be `None`.
 
 ### Ties
 
 The good news is, STAR Voting elections rarely result in a tie in the
 real world.  But ties can still happen.  The good news is, STAR Voting
 has a sensible, thorough protocol on how to break a tie.  The bad news is,
 not all ties are breakable--some ties genuinely represent the ambivalent
 will of the voters.
 
 **starvote** gives you control over how to break ties in elections,
 through the `tiebreaker` parameter to `election` and the election-specific
 functions.  **starvote** also has two predefined tiebreaker functions,
 but you can substitute your own--or none at all.
 
+The default tiebreaker in **starvote** is
+`predefined_permutation_tiebreaker`, passing
+in `candidates=None`.
+
 #### `predefined_permutation_tiebreaker`
 
 The main tiebreaker for **starvote** is
 `predefined_permutation_tiebreaker`.  This
+is a class; you should instantiate it and
+pass in the instance as the `tiebreaker`
+argument when you run the election.
+
+`predefined_permutation_tiebreaker`
 resolves the tie in favor of an ordered
-list of candidates--the candidate(s) that
-appear earliest in the list win the tie.
+list of candidates.
 
-If you don't pass in a list of candidates,
-`predefined_permutation_tiebreaker` will scan
-the ballots at the start of the election to
-produce a list of all the candidates, then
-randomly shuffle the list and use *that* list
-as the list of candidates.
-
-`predefined_permutation_tiebreaker` prints
-the permuted list of candidates at election
-initialization time, and prints its process
+Given these three variables, defined
+at the time it breaks the tie:
+
+* `candidates`, an ordered list of *all*
+  candidates participating in the election,
+* `tie`, an iterable of the tied candidates, and
+* `desired`, the number of winners we wanted.
+
+`predefined_permutation_tiebreaker` computes
+the winners of the tie as follows:
+
+```
+winners = [c for c in candidates if c in tie][:desired]
+```
+
+In other words, it returns a *desired*-length
+subset of *tie*, preferring candidates that
+appear earlier in *candidates* over those that
+appear later.
+
+`predefined_permutation_tiebreaker` accepts
+a `candidates` argument, which should be
+an ordered pre-chosen list of all candidates.
+The default value is `None`, which instructs
+`predefined_permutation_tiebreaker` to scan
+the ballots at the start of the election,
+produce its own list of all the candidates,
+randomly shuffle that list, and use that list
+as the `candidates` list.
+
+If you pass in your own `candidates` list,
+you may also pass in a string for the
+`description` keyword-only parameter, which
+should be text describing the source of
+this ordered list of candidates.
 
 #### `on_demand_random_tiebreaker`
 
-If you prefer you can use `on_demand_random_tiebreaker`
+If you prefer more unpredictability in your life,
+you can choose `on_demand_random_tiebreaker`
 to break ties.  `on_demand_random_tiebreaker` will
 simply pick a random candidate (or candidates)
 on demand, using Python's `random.sample` function.
+`on_demand_random_tiebreaker` is a function;
+you should simply pass it in as the `tiebreaker`
+parameter.
 
 #### `UnbreakableTieError`
 
 If you explicitly set `tiebreaker` to `None`,
 and an election results in a tie, `starvote` will
 raise an `UnbreakableTieError` exception.  You can
 get a text description of the tie by calling `str` on the exception;
@@ -327,15 +373,15 @@
 in the `tiebreaker` parameter to your chosen election
 function.  Custom tiebreakers can be either a function
 or a class.
 
 A custom tiebreaker function should have this signature:
 
 ```Python
-def custom_tiebreaker(options, candidates, desired, exception):
+def custom_tiebreaker(options, tie, desired, exception):
 ```
 
 Here's what these four parameters will contain:
 
 * `options` is a **starvote** `Options` object.  `options`
   has attributes mapping to the arguments you passed in to
   `election`.  You should obey `options.verbosity` when
@@ -352,27 +398,28 @@
     first (and only) positional argument.  Also accepts
     a `numbered` parameter; if `numbered` is true, it
     prints the candidates in order, prepended by their
     ordinal number (starting with 1).  If `numbered` is
     false, `print_candidates` attempts to sort the
     candidates before printing them.
 
-* `candidates` is a list of the tied candidates.
+* `tie` is a list of the tied candidates.
 
 * `desired` is the desired number of winners.
 
 * `exception` is the `UnbreakableTieError` for this
   tie.  If you can't break the tie, you should raise
   this object.
 
-Note that **starvote** will parse the tiebreaker function's
-docstring.  The first line of the docstring will be used
-as a "heading" printed during election initialization, with
-the rest of the docstring printed as the body of that heading
-if `options.verbosity` is 1 or greater.
+Note that **starvote** will also parse the tiebreaker
+function's docstring.  The first line of the docstring
+will be used as a "heading" printed during election
+initialization, with the rest of the docstring will be
+printed as the body of that heading if `options.verbosity`
+is 1 or greater.
 
 You can also write a custom tiebreaker class.  The only
 requirement is that the class inherits from
 `starvote.Tiebreaker`, and it supports a `__call__` method
 with the same signature as a custom tiebreaker function.
 (However, here the docstring is ignored; it's up to you
 to call `options.heading` and `options.print`.)
@@ -420,37 +467,37 @@
 Git repo.)
 
 After this example code finishes,
 the `winners` variable will contain the list `['Chuck']`.
 The example also produces this output:
 
 ```
-[STAR]
+[STAR Voting]
   Tabulating 3 ballots.
   Maximum score is 5.
-[STAR: Initializing ordered permutation tiebreaker]
+[STAR Voting: Initializing ordered permutation tiebreaker]
   Computing a random permutation of all the candidates.
   Permuted list of candidates:
-    1. Chuck
-    2. Amy
-    3. Brian
+    1. Brian
+    2. Chuck
+    3. Amy
   Tiebreaker candidates will be selected from this list, preferring candidates with lower numbers.
-[STAR: Scoring Round]
+[STAR Voting: Scoring Round]
   The two highest-scoring candidates advance to the next round.
     Chuck -- 13 (average 4+1/3) -- First place
     Amy   -- 10 (average 3+1/3) -- Second place
     Brian --  9 (average 3)
   Chuck and Amy advance.
-[STAR: Automatic Runoff Round]
+[STAR Voting: Automatic Runoff Round]
   The candidate preferred in the most head-to-head matchups wins.
     Chuck         -- 2 -- First place
     Amy           -- 1
     No Preference -- 0
   Chuck wins.
-[STAR: Winner]
+[STAR Voting: Winner]
   Chuck
 ```
 
 
 ### *starvote format*
 
 `starvote` also defines a custom text format for specifying
@@ -741,14 +788,21 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.2** - *2023/05/27*
+
+* Renamed the `tiebreaker` parameter `candidates` to `tie`.
+* Evicted some testing-only tiebreakers from the `starvote`
+  module.  They're now in their own script, which only gets
+  loaded when working with the test suite.
+
 **2.0.1** - *2023/05/27*
 
 * Changed the nickname of the reference version of
   Allocated Score Voting to "Allocated-R".
 
 **2.0** - *2023/05/27*
```

