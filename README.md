  test "CRC check method returns true for valid VST_PAT tokens" do
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("cfdgksmyyogbj6b6k7tvu6wfgotk453xxadybrrs22g6qekcaw3y")
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("cfdgksmyyogbj6b6k7tvu6wfgotk453xxadybrrs22g6qekcaw3x")
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("67csyuknm2k4azb2q3ktjb7dwnafo2xj5bwpv7vt7ei2l5a7wwfb")
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("nj3ithqqxdghjtxuo6a27lebc4ko5jyqsthyqshtnnlpvowh2oaq")
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("36tbhyubwbvmi3xzek5n7gz2mxxx3ywxoujzjoxtb3ptgdyfauia")
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("r5cd6wmuyil22fwl7yy7tukhtkr5dh3ex6eaw6qmtbfdikdvjlvq")
    assert_equal true, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("xwejwqtlcznyx5ateua3232d3iq4xx2zt3dinyqyvmvk4my6ctfq")
  end
  
  test "CRC check method returns false for invalid VST_PAT tokens" do
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("67csyuknm2k4azb2q3ktjb7dwnafo")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("xwejwqtlcznyx5ate")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("67csyuknm2k4azb2q3ktjb7dwnafo2xj5bwpv7vt7ei2l5a7wwf")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("67csyuknm2k4azb2q3ktjb7dwnafo2xj5bwpv7vt7ei2l5a7wwfr")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("r5re6wmuyil22fwl7yy7tukhtkr5dh3ex6eaw6qmtbfdikdvjlvq")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("xwuiwqtlcznyx5ateua3232d3iq4xx2zt3dinyqyvmvk4my6ctfq")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("advancedthreatprotectiononboardingdevicesettingstate")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("windowsinformationprotectionpincharacterrequirements")
    assert_equal false, GitHub::TokenScanning::TokenScanningPostProcessingHelper.valid_vsts_pat_crc?("deviceenrollmentwindowshelloforbusinessconfiguration")





http://test.blob.core.windows.net/test/test.vhd?sr=c&si=test&sig=abcdefghijklmnopqrstuvwxyz0123456789%F%2BABCDE%3D

http://test.blob.core.windows.net/test/test.vhd?sr=c&si=test&sig=abcdefghijklmnopqrstuvwxyz01234569%F%2BABCDE%3D

http://test.blob.core.windows.net/test/test.vhd?sr=c&si=test&sig=abcdefghijklmnopqrstuvwxyz012345678%F%2BABCDE%3D
