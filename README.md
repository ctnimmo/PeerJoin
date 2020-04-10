# PeerJoin
PeerJoin stuff

var D = 2; // Change this to desired distance

var psiX = latX.toRadians();
var thiX = lonX.toRadians();

var lonDist = D / Math.cos(psiX);

var thiUpper = thiX + lonDist;
var thiLower = thiX - lonDist;

var lonUpperDegrees = thiUpper.toDegrees();
var lonLowerDegrees = thiLower.toDegrees();

Use lonLowerDegrees and lonUpperDegrees to determine cut-off points.
